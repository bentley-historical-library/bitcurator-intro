---
title: 'Reporting'
teaching: 5
exercises: 3
---

:::::::::::::::::::::::::::::::::::::: questions 

- What tools are available in the BitCurator environment for analyzing disk images and data tranferred from legacy media?
- How can librarians and archivists capture basic system characteristics and metadata?
- How can they scan for for potentially sensitive information?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Gain experience with:
  - Brunnhilde, a reporting tool for directories and disk images;
  - `bulk_extractor`, which scans for credit card numbers, emails, etc.; and
  - fiwalk, to print filesystem statistics
- Locate the BitCurator Quick Start Guide and other resources detailing reporting functionality in the BitCurator Environment.

::::::::::::::::::::::::::::::::::::::::::::::::

_Note: If you haven't yet created a disk image or otherwise have data to work with, you can download sample data from BitCurator's Github site and work with that: [bcc-dfa-sample-data](https://github.com/bitcurator/bcc-dfa-sample-data). You can clone the repository or download and unzip the file._

## Mounting and Examining a Disk Image

If starting with a disk image, you'll first need to mount it in order to analyze the files on it. BitCurator contains some convenience scripts to automatically mount disk images.

Right-click on a disk image from Files, and then click "Disk Image Mount" from "Scripts." If everything works, you should see it appear as a mountable device in the list of the left. You can then navigate the files and explore them.

_Note: This mount is read-only._

## Reporting

BitCurator includes a variety of tools to analyze and report on disk images and the filesystems they contain.

### Analyzing a Disk Image with Brunnhilde

One such tool is Brunnhilde, a Seigfried-based characterization tool for directories (and disk images). Open up the Terminal, and use the command `brunnhilde.py --help` to view Brunnhilde's usage information. Alternatively, you can find Brunnhile from the Applications menu.

### bulk_extractor and Bulk Reviewer

#### Scanning Disk Images and Directories with Bulk Reviewer

#### Scanning Disk Images, Files, and Directories with bulk_extractor

## fiwalk

## Additional resources
