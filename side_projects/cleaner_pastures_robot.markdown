---
layout: page
title: Cleaner Pastures Robot
hero_height: is-small
permalink: /cleaner_pastures_robot/
---

## Abstract
Team Cleaner Pastures is a student group project from Introduction to Robotics focused on implementing simple object sorting within the CoppeliaSim robotics simulation platform. The importance of this is to provide a proof of concept for a potential trash sorting robot, with every piece of the setup except the sorting algorithm itself simulated accurately. In our project we sorted between red and green cubes, but in the real world this would simply be replaced with trash and recyclable objects - which the robot could be trained on with neural networks. Our robot’s main solution is to use a proximity sensor to let the conveyor belt setup know when to stop, at which point the robot picks up a block and uses a vision sensor to move the block to the desired location. To measure our success, we let our simulation run several times and noticed a 90.16% success rate. Qualitatively, we felt pretty satisfied with our results, because we were able to sort the overwhelming majority of blocks. Overall, this project was a great exercise in understanding what work goes into creating a robotics system besides just programming. In the real world, sensors may malfunction and other unexpected things may happen, so those are areas to explore in the future.

## Report
The final report for this project can be found [here](/docs/cleaner_pastures_report.pdf).

## Demo & Project Links
<p align="center">The following images link to the ECE 470 course page, final demo video, and GitHub repository for the project.</p>

<div class="columns is-mobile is-multiline is-centered is-vcentered">
    <div class="column is-narrow">
        <p>
            <a href="https://publish.illinois.edu/ece470-intro-robotics/"><img src="/img/uiuc_ece.jpg" alt="ECE 470 Website" width="200" /></a>
        </p>
    </div>
    <div class="column is-narrow">
        <p>
            <a href="http://www.youtube.com/watch?v=pLc1tVorXGs"><img src="http://img.youtube.com/vi/pLc1tVorXGs/0.jpg" alt="Cleaner Pastures Final Demo" /></a>
        </p>
    </div>
    <div class="column is-narrow">
        <p>
            <a href="https://github.com/vyomthakkar/ece470finalproject"><img src="/img/github.png" alt="Github Project" width="200" /></a>
        </p>
    </div>
</div>

## Introduction
The objective of our project is to make use of the UR3 robot arm, a gripper, and two sensors in order to make a sorting robot. We pitched the robot in our final project video as a consumer product, but a more realistic use case would perhaps be to sort objects that get taken to garbage dumps, as often recyclable objects are mistakenly thrown away. Coming into this project, our team was familiar with python but thoroughly unfamiliar with robotics simulation or CoppeliaSim. In order to solve our task, we did research on how to connect the python remote API as well as on LUA scripting . We also needed to use our knowledge from lectures to implement a functional forward and inverse kinematics system for our robot arm. For equations, we consulted the Modern Robotics Textbook. Finally, for vision sensing, we consulted Coppelia's website.

## Modules
<p align="center"><img src="/img/470_modules.jpg" alt="Module Block Diagram" /></p>

#### Robot Central Logic
This encompasses the decision making process of the robot, and the necessary calculations behind forward & inverse kinematics of the positioning of the arm. 

#### Vision Sensor
The camera is used to take snapshots of the block the robot is currently attempting to pick up. Specifically, the camera is an orthographic vision sensor which passes a square image input to the Robot Central Logic in order to make decisions of where to proceed.

#### UR3 Arm
The specific robot we used for Team Cleaner Pastures was the UR3 arm with six revolute joints. This decision had to be considered in the calculation of transformation matrices in our robot central logic.

#### Proximity Sensor & Conveyor Belt
The final part of the system is the standalone conveyor belt + proximity sensor module. Red and green blocks move down the conveyor belt at a speed of 0.05 m/s, and stops when the proximity sensor identifies a block cut through it. This signals to the robot central logic to begin moving to the conveyor belt.

