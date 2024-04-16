---
title: 'Disk Imaging'
teaching: 20
exercises: 1
---


:::::::::::::::::::::::::::::::::::::: questions 

- What is a disk image?
- When would you disk image media?

::::::::::::::::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::: objectives

- Use the Guymager disk imaging software to acquire the contents of a storage device and its associated metadata.
- Learn to evaluate when to image a disk based on individualized criteria. 
::::::::::::::::::::::::::::::::::::::::::::::::

## What is a Disk Image?

A **disk image** a bit-perfect sequence of all the bits on a particular physical device; in other words, a complete bitstream (as defined by the physical limits of a storage device).

  - You may have seen .dmg, or .iso files - these are images (like a thumb drive, CD, diskette)
  - We will work with “forensic images,” specifically the “Expert Witness” format (aka .E01 or EWF), which is a complete sequence of a physical drive, does not allow any modifications  

## To image or not to image?
### Considerations for disk imaging

There is no right or wrong answer to whether or not you should image a disk! 

- Are you choosing between extracting files and/or chunks of content?
- Collection considerations: 
  - What is your collecting purpose? 
  - What is the role of the device(s)?
  - What are you storage concerns?
- Device considerations:
  - What devices have an OS (that means lots of redundant & proprietary files)? 
  - If it’s a storage device, may have deleted/unintended files (these are captured by forensic imaging approaches)
  - What is on the device? Sometimes the device contents will determine if a disk image is required, such as executable files or other software.
  - What are the preservation needs?
  

## Creating a disk image

For this walk through we will be using 3.25 inch floppy disks. Similar concepts are applicable to other storage mediums, but the exact steps may differ.

### Using Guymager

<!-- insert instructions on how to use guymager and screenshots -->


#### Some disk image formats you may see
- RAW and Split RAW (RAW stored across multiple files)
- Advanced Forensics Format (AFF) [no longer recommended]
- EnCase Evidence File (.E01)
- ISO (for CD-ROM)
- IMG (floppy or sometimes CD-ROM)

##### RAW format (dd)
- Copies of the raw media data. Often split into smaller chunks to make them more  manageable and so that the resulting images can fit onto limited file systems and  media such as FAT or DVD/CDROM.
- Advantages:
  - Very simple, use simple tools to manipulate the image.
  - Image can be easily split for storage and transport on removable media
  - Output can be piped to other applications for immediate processing
- Disadvantages:
  - Can be very large (no compression). Zipped raw images cannot be  operated on directly with regular tools (efficiently perform arbitrary seeks).
  - Often too large to store on FAT formatted media
  - No metadata other than file names, no hashes.
  - No checksumming on files – not robust
  - Missing segments (for example from scratched CD/DVD – can  sometimes be overwritten with 0’s).
  - Overwritten data (unrecoverable – no checksums on small blocks in  file).
  
##### Expert Witness Format (EnCase)
- Evidence file consists (in order) of: Acquisition information, Data Block, CRC (cyclic redundancy check), acquisition hash (MD5)
- Can be split for storage, transport
- CRC computed for every 32K block; balance between integrity and  speed, also makes it very difficult to tamper with the evidence file (1 in 4 billion chance of collision)
- Cannot be manipulated with simple (open source UNIX) tools; support  reverse engineered in libewf
- Previously limited to 2GB size
- Largely proprietary
- Has been reverse engineered by Joachim Metz in libewf (used in open source tools that read EWF) - (http://sourceforge.net/projects/libewf/files/) 

##### ISO (.img) for CD-ROM, DVD
- Similar to raw, but can’t contain 
  - multiple tracks
  - audio or video tracks
- Doesn’t contain control headers or error correction fields (raw can include these)
- Filesystem usually will be either ISO 9660 (CD-ROM) or UDF (DVDs)

### Accessing Disk Images

- Virtualization and emulation
- Mounting the original filesystem
- Accessing (but not mounting) disk images using forensics software
- For end user access:
  - Remote, dynamic access to disk image contents (via server, virtual environment)
  - Cross-drive analysis

### Mount disk image: Using BitCurator Mounter

<!-- insert instructions on how to mount an image and screenshots -->
  
::::::::::::::::::::::::::::::::::::: Do it Yourself!

Two activity options:
1. Create your own image from the supplied 3.25 inch floppy disks. 
2. Use one of the already created disk images available in the [GitHub repo] (https://github.com/BitCurator/bcc-dfa-sample-data).

Try to mount the disk image your created or downloaded. 

What information do you see?

:::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: keypoints 

- Digital forensic approaches can offer useful tools to digital curators in working with legacy removable media
- Important concepts include thinking beyond the file level and disk imaging
- BitCurator environment offers a useful bundle of tools that are of use to digital curators

::::::::::::::::::::::::::::::::::::::::::::::::



