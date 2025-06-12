---
title: Kernel Module Programming
date: 2025-04-17
author: MUGUREl
description: Kernel Driver Programming is a guide for setting up and debugging kernel modules.
isStarred: false
---
# What is kernel?

# What is kernel module?

# Initial setup for debugging


# Commands about kernel modules
- lsmod # List loaded kernel modules
- modinfo <module_name> # Show information about a kernel module
- insmod <module_name> # Load a kernel module
- rmmod <module_name> # Unload a kernel module
- dmesg <module_name> # Show messages from a kernel module
- dmesg -W # wait for new messages
- dmesg -w # Show all pass messages from a kernel module and wait for new messages
- modprobe <module_name> # Load a kernel module and its dependencies
