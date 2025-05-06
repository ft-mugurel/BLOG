---
title: VKM
date: 2025-04-17
author: MUGUREl
description: Vuln 1001 course notes
isStarred: false
---
# Initial setup for debugging
- We need an kernel with debugging enabled.

1. Install the linux kernel.
``` bash
git clone --depth 1 --branch v6.12 https://github.com/torvalds/linux.git
cd linux
```

2. Create the default configuration file.
``` bash
make defconfig
```

3. Enable the following options:
``` bash
make menuconfig

// -- the potion to enable 
Kernel hacking  --->
    Memory Debugging  --->
        [*] KASAN: runtime memory debugger
        [*]   KASAN: Generic mode
```

4. Compile the kernel.
``` bash
make -j$(nproc)
make modules -j$(nproc)
make INSTALL_MOD_PATH=../modroot modules_install
```

4. Create and minimal file system
``` bash
git clone https://git.busybox.net/busybox
cd busybox
make defconfig
make menuconfig // disable tc
make -j$(nproc)
make CONFIG_PREFIX=../modroot install
```
# What is kernel module?
- A kernel module is a piece of code that can be loaded into the kernel at runtime, allowing for dynamic extension of the kernel's functionality.
