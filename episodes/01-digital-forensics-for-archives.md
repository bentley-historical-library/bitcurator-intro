---
title: 'Digital Forensics for Archives'
teaching: 5
exercises: 3
---

::::::::::::::::::::::::::::::::::::::: objectives

- Become familiar with digital forensics techniques and their application in cultural heritage and digital curation
- Identify and understand various types of magnetic disk removable media, which might be encountered in collections
- Describe and recommend tools and techniques for extracting content from legacy media, including use of write blockers and creation of disk images
- Understand various types of metadata that can be generated for born-digital content extracted from legacy media
Become familiar with BitCurator and its toolset

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- Why might archivists, librarians, and other cultural heritage workers want to use digital forensics techniques and tools?
- What are some known use cases of digital forensics usage amongst archivists, librarians, or others?
- What is BitCurator? What is the BitCurator environment? Is it the same as "digital forensics"?

::::::::::::::::::::::::::::::::::::::::::::::::::

## Digital Forensics

Digital forensics refers to a suite of activities and tools to preserve
the original context of digital materials (e.g., the system timestamps and OS structure)
and extract content at the bitstream level from damaged or deleted digital content.

## Archivists + Digital Forensics: Why

What are some use cases for digital forensics with legacy born digital materials?

:::::::: discussion

Why are you interested in digital forensics for archives and other cultural heritage collections?

What potential uses for these tools are you considering in your context?

::::::::

## Enter BitCurator Environment (BCE)

To address this, a group of archivists and researchers developed the BitCurator Environment, or BCE.
The BCE is a suite of open-source digital forensics softwares that are particularly useful to archivists in tracking creation metadata, structure, file identification, and documenting provenance. It even contains some built-in writeblockers and other tools to preserve original order and chain of custody.
BitCurator tools are grouped within an Ubuntu-based Linux environment and can be run virtually
or installed directly as the main OS of a workstation, and together this is all known as the BCE.
We will discuss BCE more in the next episode.

## Resources

There are many resources that explain how to use
the BCE and other digital forensics tools.
Given that this lesson focuses on BCE,
most of the resources are geared toward this software
environment, but the list also includes a few more general resources:

- [BitCurator Docs](https://bitcurator.github.io/documentation/) - overview and explanation of all current BCE tools and functionalities
- Corinne Rogers, “From time theft to time stamps: mapping the development of digital forensics from law enforcement to archival authority,” _International Journal of Digital Humanities_ (2019): 13–28. DOI: [10.1007/s42803-019-00002-y](https://dx.doi.org/10.1007/s42803-019-00002-y)
- Julianna Barrera-Gomez and Ricky Erway, “Walk This Way: Detailed Steps for Transferring Born-Digital Content from Media You Can Read In-house,” 2013, OCLC Research. Available at [https://www.oclc.org/content/dam/research/publications/library/2013/2013-02.pdf](https://www.oclc.org/content/dam/research/publications/library/2013/2013-02.pdf)
- Christopher A. Lee, et al., “From Bitstreams to Heritage: Putting Digital Forensics into Practice in Collecting Institutions,” whitepaper for BitCurator, September 2013. Available at [https://bitcurator.net/wp-content/uploads/sites/1099/2018/08/bitstreams-to-heritage.pdf](https://bitcurator.net/wp-content/uploads/sites/1099/2018/08/bitstreams-to-heritage.pdf)
- Sam Meister and Alexandra Chassanoff, “Integrating Digital Forensics Techniques into CuratorialTasks: A Case Study,” International Journal of Digital Curation 9 (2014): 6-16. DOI: [10.2218/ijdc.v9i2.325](https://dx.doi.org/10.2218/ijdc.v9i2.325)

:::::::: keypoints

- Digital forensics identifies a range of activities which aim to extract and preserve contextual information about digital content on external devices, like laptops, servers, drives, and even legacy devices like floppy disks and USB drives
- Digital forensics tools and techniques can help digital preservation work, particularly in maintaining information about original order, provenance, and chain of custody for digital objects
- Digital preservation workers, particularly archivists, have used digital forensics techniques and tools to record information about, process, and preserve digital content, and particularly to address content stored on legacy digital devices

::::::::