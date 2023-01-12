---
layout: page
title: Human Interactive Self Balancing Security Robot
hero_height: is-small
permalink: /xe_security_bot/
---

## Abstract
The purpose of this project is to create a self-balancing robot that can roam the hallways of a school and identify people who shouldn’t be on campus. This is being accomplished through three main production steps: (1) Hardware aspect of building frame and hooking up electronics, (2) Programming self-balancing code of for wheels of robot, (3) Programming face detection and face recognition code through OpenCV. This robot would ensure a safer environment on campus. This was a high school senior project completed under Dr. George Kantor at the Robotics Institute of Carnegie Mellon University with two fellow students: Edward Fitzpatrick & Amir Megherhi.

## Report
The final report for this project can be found [here](/docs/xe_robot_report.pdf).  
The poster can be found [here](/docs/xe_robot_poster.pdf).  
And the final presentation can be found [here](/docs/xe_robot_presentation.pdf)

## Original CAD Design & Hardware Build
<div class="columns is-mobile is-multiline is-centered is-vcentered">
    <div class="column is-narrow">
        <p><img src="/img/xe_robot_cad_orig.PNG" alt="Original CAD" width="400" /></p>
    </div>
    <div class="column is-narrow">
        <p><img src="/img/xe_robot_first_build.jpg" alt="Original Build" width="400" /></p>
    </div>
</div>

Initially, a CAD model was developed to consider how to build the base of the robot housing motors & controllers, gear boxes, a Raspberry Pi, and a battery. This first model takes inspiration from the development of [ZeGoBeast](/zegobeast), with the housing walls made up of plywood. This translated into a first design build by laser cutting side panels, and putting electronics within it. 

## Electronics
<div class="columns is-mobile is-multiline is-centered is-vcentered">
    <div class="column is-narrow">
        <p>
            <img src="/img/xe_robot_pwm_block.jpg" alt="Block Diagram of Electronics" width="500" />
        </p>
    </div>
</div>
<div class="columns is-mobile is-multiline is-centered is-vcentered">
    <div class="column is-narrow">
        <p>
            <img src="/img/xe_robot_electronics.jpg" alt="First Revision of Electronics" width="200" />
        </p>
    </div>
    <div class="column is-narrow">
        <p>
            <a href="http://www.youtube.com/watch?v=yFSmZc3EVr0"><img src="http://img.youtube.com/vi/yFSmZc3EVr0/0.jpg" alt="Original Base of Security Bot Design" /></a>
        </p>
    </div>
</div>

A circuit was built with the Raspberry Pi as the primary computation power house. The Raspberry Pi was programmed to send Pulse Width Modulation (PWM) signals to Talon motor controllers in order to power the motors accordingly. A module was installed on the Pi to take in Xbox 360 controls, which in turn spun the motors depending on joystick inputs. All of these electronics were powered with a power distribution board. The image on the right can be clicked to view a demo of the initial remote controlled motors.

## Next Base Revision
<div class="columns is-mobile is-multiline is-centered is-vcentered">
    <div class="column is-narrow">
        <p><img src="/img/xe_robot_cad_new.PNG" alt="New CAD" width="400" /></p>
    </div>
    <div class="column is-narrow">
        <p><img src="/img/xe_robot_new_frame.jpg" alt="New Frame" width="400" /></p>
    </div>
    <div class="column is-narrow">
        <p><img src="/img/xe_robot_new_build.jpg" alt="New Build" width="400" /></p>
    </div>
</div>

After experimenting with the original base, we identified it was not going to be sturdy in the long term, and we developed a new CAD model with bars and plexiglass shieldings to house the contents. This was then machined into existance. 

## Face Recognition
The Eigenface baseline algorithm built into OpenCV was used to crossreference a stored data base of student faces, and recognize people who appeared in front of the robot's on-board camera module. The computation was completed on the Raspberry Pi which led to severe limitations in real time calculations as the processor was not powerful enough. In reality, these computations should be sent to a cloud computing platform which could identify people much quicker.
