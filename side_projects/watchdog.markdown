---
layout: page
title: Project LD & Watchdog Accelerated Security Camera
hero_height: is-small
permalink: /watchdog/
---

## Abstract
Project LD (Legends Never Die) is my partner's and my final project for Digital Systems Laboratory at the University of Illinois. We developed a hardware accelerated 2D match moving core on a DE2-115 Development Board equipped with Intel's Cyclone IV E FPGA. Our original inspiration was to develop an augmented reality beer pong experience to users (without the beer 😉). Some considerations we made during the design process include integration with a camera module, USB mouse, & VGA monitor, software/hardware implementations of 2D tracking alorithms, and the finite state machine of the entire system. While we did not develop the 3D module, we provide our conceptual ideas for how to go about the problem in our final report. This continued as an entry into InnovateFPGA 2019 as linked at the end of this page.

## Report
The final report for Project LD can be found [here](/docs/ld_report.pdf).

## Demo & Project Links
<p align="center">The following images link to the ECE 385 course page, final demo video, and GitHub repository for the project.</p>

<div class="columns is-mobile is-multiline is-centered is-vcentered">
    <div class="column is-narrow">
        <p>
            <a href="https://ece.illinois.edu/academics/courses/ECE385"><img src="/img/uiuc_ece.jpg" alt="ECE 385 Website" width="200" /></a>
        </p>
    </div>
    <div class="column is-narrow">
        <p>
            <a href="http://www.youtube.com/watch?v=chocc--7Fws"><img src="http://img.youtube.com/vi/chocc--7Fws/0.jpg" alt="Project LD Final Demo" /></a>
        </p>
    </div>
    <div class="column is-narrow">
        <p>
            <a href="https://github.com/harris-mohamed/Project-LD"><img src="/img/github.png" alt="Github Project" width="200" /></a>
        </p>
    </div>
</div>

## Modules

#### VGA
A VGA monitor is used to display the tracking visually to the user. Altera's VGA Controller IP sends vertical/horizontal sync signals as well as the pixel color value to the monitor at every position to output frames. As counter scans from left to right and from top to bottom through the monitor, a defined Color Mapper module sends the specific color value that needed to be drawn at that specific location. This is how the tracking box, blue filtering pixels, and mouse position were drawn to the screen.

#### Camera
The camera module utilized was Altera's TRDB_DC2 1.3 mega pixel sensor, and was one of the most difficult portions of the system to interface with. This is a charge-coupled device image sensor which charges capicators as light hits the sensor, and stores color data accordingly. The data that is taken from the camera cannot be received parallely as a result, and we had to develop modules to extract pixel values sequentially instead. Each camera clock cycle, a pixel is grabbed from the camera and passed through several filters and pipelines before finally being output to the tracking module and VGA monitor. 

#### System on Chip & Software
We utilized Intel's Nios II/e soft processor to interface camera gain settings and the USB mouse. Because there is only one SDRAM controller on board used for the camera, the soft processor was stored trough on-chip memory, which ensures the speed of the processor is the fastest. This processor fed data to the FPGA about mouse coordinates, and initial user settings for the gain of the camera with code written in C. 

#### System FSM
The finite state machine for the project is a Mealy Machine which transitions via mouse inputs from a user initialization phase, to an inital ball localization input, to a ball tracking phase.

#### 2D Tracking
A Tracker module was developed in hardware to identify and track the location of the ping pong ball with 2D match moving. As the VGA signal scans from left to right and top to bottom, the pixel is passed to the tracker module. If the current pixel is found to be within a margin outside or inside of the current estimation of the tracked location of the ball and is within a defined color threshold for the ball, the tracking box expands or shrinks accordingly. This results in the tracking box moving as the ball moves in the real world. 

## Project Watchdog
Project LD continued as Project Watchdog submitted to InnovateFPGA 2019, where my partner & I received regional finalist standing. More details about that project can be found [here](https://web.archive.org/web/20200923182208/http://www.innovatefpga.com/cgi-bin/innovate/teams.pl?Id=AS020).

