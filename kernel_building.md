---
title: Kernel Building
layout: page
---

# Initial Setup

Follow this guide from the Raspberry Pi documenation: [here](https://www.raspberrypi.org/documentation/linux/kernel/building.md)

This will setup most of what you need in regards to tooling and configuration for kernel setup.

# The .config
This set will configure the kernel with extra or any other settings that you may desire. To initially set it up:

` $ sudo apt-get install libncurses5-dev `

Then run the following command to setup the default configuration for the Raspberry Pi 2(configure for the ARM7 BCM2709 processor).

` $ make bcm2709_defconfig `

### Using menuconfig

Then to configure the default `.config` file that is created after the above step.

` $ make menuconfig `

After a bit of compilation, there will be a menu system that will prompt a bunch of submenus that will much more in depth configuration of the kernel with help messages for each flag.

Make sure to save the `.config` file after tweaking the kernel!

# Building

See back to the [Build](https://www.raspberrypi.org/documentation/linux/kernel/building.md) from the Raspberry Pi Documentation. This has building instructions for cross-compiling and local building on a Raspberry Pi.

# Extras

Some extra kernel configurations:

- No [ARM MMU](https://en.wikipedia.org/wiki/Memory_management_unit) processor support: [.config](https://gist.github.com/DevinCarr/cdeed3fa76ffca0dedc9)
- Could configure an optimized build for multi-core and uni-core processors. (Even though the Raspberry Pi 2 has a multi-core processor, it could be shown to slow down with kernel support for one core)
  - Enabling the scheduler to work one core or even a different scheduler could be found possibly in here.
