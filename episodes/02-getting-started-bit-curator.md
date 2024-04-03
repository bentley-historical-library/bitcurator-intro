---
title: 'Getting Started with BitCurator'
teaching: 5
exercises: 3
---

:::::::::::::::::::::::::::::::::::::: questions 

- How do I install and use digital forensics tools that may be useful for digital curation activities?
- What is a disk image and how can I create one?
- What tools may be used to acquire born-digital materials from removable storage media (and other locations), which ensure the integrity of the data, create useful information about the source and the resulting materials, and can help to preserve the context of the original materials? 
- What sorts of digital media are most well suited to this sort of activity? Are there some that are not?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Test and evaluate tools for use in the identification, transfer, and preservation of born-digital materials.
- Install and become familiar with the tools in the BitCurator environment.
- Identify appropriate tools for acquiring born-digital content from removable media and scan for potentially sensitive information stored in that media. 
- Use the Guymager disk imaging software to acquire the contents of a storage device and its associated metadata.

::::::::::::::::::::::::::::::::::::::::::::::::

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

## Activities

::::::::::::::::::::::::::::::::::::: challenge

## Getting around in BitCurator

Getting around - tasks

:::::::::::::::::::::::: solution

## Solution
 
Getting around: Answers will vary, depending on what you choose to look at. 
At minimum, you should look at the various "Applications" (menu up at the top),
use the right click option to look at file information, checksums, and 
look around to find other interesting things.


::::::::::::::::::::::::
:::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: keypoints 

- Use BitCurator as a helpful way to bundle together and run many tools useful to 
digital forensics that are appropriate to digital curation. That is, tools that assist
in creating trustworthy digital copies, provenance information, contextual data,
and chain of custody information.
- You can use `GuyMager` to make disk images.
- BitCurator has things set up so you can use `GuyMager` as well as other tools that
will document your transfer and copying processes. 

::::::::::::::::::::::::::::::::::::::::::::::::
