---
layout: page
title: LC4 Operating System
hero_height: is-small
permalink: /lc4/
---

## Abstract
The LC4 is an operating system developed as a final project Computer Systems Engineering at the University of Illinois. The design process spanned approximately eight weeks where, as a group of four, we wrote necessary code to initialize the processor (Interrupt Descriptor Table, Global Descriptor Table, devices, and paging), wrote device drivers (terminal, file system, and real time clock), implemented system calls and tasks, and finally implemented round-robin scheduling. project pushed us to collaborate and perform code reviews together, and experience a similar workload to the real world where we will have to parse dense documentation, debug code together, and use best practices. The course doesn't allow us to provide direct access to code to others for academic integrity reasons, but demos and videos are provided in following sections.

## Demo & Project Links
<p align="center">The following images link to the ECE 391 course page & final demo video.</p>

<div class="columns is-mobile is-multiline is-centered is-vcentered">
    <div class="column is-narrow">
        <p>
            <a href="https://ece.illinois.edu/academics/courses/ece391"><img src="/img/uiuc_ece.jpg" alt="ECE 391 Website" width="200" /></a>
        </p>
    </div>
    <div class="column is-narrow">
        <p>
            <a href="http://www.youtube.com/watch?v=ARYjKrD7jYs"><img src="http://img.youtube.com/vi/ARYjKrD7jYs/0.jpg" alt="LC4 Operating System Final Demo" /></a>
        </p>
    </div>
</div>

## Tasks of Project I Owned
Rather than discussing the inner-workings of every module in the LC4, I'll go through an overview of the portions of the project I took ownership of. This primarily consisted of memory related modules like paging, video mapping, & file system protocols. 

#### Paging
<p align="center"><img src="/img/paging.png" alt="Paging Design Iteration" width="600" /></p>

Paging is one form of virtualization in operating systems, and makes it seem like there is more memory available to the user than there really is. Paging structures come in the form of directories and tables which convert a virtual address provided by the user to a physical address on RAM. In modern operating systems, page directories and tables are dynamically allocated and destroyed as memory is used up by users and programs. In this project, we were told there will be a maximum of six programs running at any time, so I made the design choice to statically allocate memory to necessary paging structures at boot time. As programs get switched out by the scheduler, the CR3 register points to the respective page directory of the running program. 

#### Video Mapping
<p align="center"><img src="/img/fish.gif" alt="Video Mapping Output Example" width="600" /></p>

One of the system calls that we needed to make available to the user was a video mapping function, which would allow the user to draw directly to the terminal screen. This is different from printing text to the screen with the terminal driver because programs should be able to draw to any place on the terminal. This required keeping track of the state of the page directories when switching between programs, and remapping the physical address that the user receives when running a vidmap program. Above is a GIF of the fish program running on one of the three terminals, which uses video mapping.

#### File System
<p align="center"><img src="/img/file_sys.png" alt="File System Storage" width="600" /></p>

The provided file system stored consists of blocks of an initial boot block with details of the counts of the number of directory entries and similar details, inodes with contents holding file size and pointer data for each file in the system, and data blocks with actual data for each file. In this project, we had to implement read only parsing functionality for the file system. This was done by developing dentry, boot_block, & inode data types, and writing file system initialization, dentry searching, data extraction functions. Another functionality that had to be added was to load new programs and switch the page directory pointers as the scheduler switched from one task to another.
