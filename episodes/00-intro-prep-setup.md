---
title: 'Setup'
teaching: 5
exercises: 3
---

Here's how to setup BitCurator

## Instructions

For this lab, the main goal is to get started with BitCurator. To do this, you will need to install BitCurator on your local computer, and you will also need to have a small removable storage device, such as a USB drive or thumb drive. (Your removable storage media should be modest in capacity in order to reduce file sizes.) 

The overall steps in this task are as follows:

1. Install BitCurator locally (on your laptop, or a desktop that you use and have access to). This will require installing VirtualBox, which is a software from Oracle, an "image" of BitCurator to use for importing the image to VirtualBox, and then starting up the BitCurator environment on your computer.
1. Launch BitCurator in the VirtualBox environment, and spend some time getting familiar with
the tool's in the BitCurator environment.
1. Acquire a disk image of some sample of digital materials (from a USB or small
storage device) using GuyMager, a disk imaging tool that is part of the BitCurator 
environment.

For reference, these are the tools you will be focused on:

* [BitCurator](https://github.com/BitCurator/bitcurator-distro/wiki/Releases) - as of January 2023, the current version is 4.4.1 
* [GuyMager](https://guymager.sourceforge.io/) (note that this is already part 
of the above, so there is not need to install it separately)

## Installation Tips

* To guide your BitCurator installation and imaging process, you should consult
Bitcurator's QuickStart Guide, available here: http://distro.ibiblio.org/bitcurator/docs/BitCurator-Quickstart-v4.x.x.pdf.
* Note that for this activity, **you will be using the "Virtual Appliance" option, not the option to 
install as a direct boot or partition**. So, you do not need to create a bootable 
USB drive prior to installation (ignore instructions about that). 
* You can use the `.ova` file linked here for your virtual appliance: https://distro.ibiblio.org/bitcurator/BitCurator-4.4.1.ova ([SHA256 for verification](https://distro.ibiblio.org/bitcurator/BitCurator-4.4.1.ova.sha256))
* Be sure to **set up a Shared Folder** as outlined in the instructions, so that you can save files to your local computer (outside the VM). 
* If you are ever asked while using BitCurator to enter an **administrator password**, 
use **bcadmin**.