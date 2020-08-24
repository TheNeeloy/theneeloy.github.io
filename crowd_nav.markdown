---
layout: page
title: Robot Navigation in Crowded Environments
hero_height: is-small
permalink: /crowd_nav/
---

## Purpose
In real world situations, a robot may find itself having to navigate safely through crowds or between obstacles before getting to its orginal goal. In this circumstance, it's critical that the robot does not collide with other masses to avoid unintentional confrontation or damage. Current state of the art algorithms for crowd navigation (ORCA, CADRL, SARL, etc.) do not necessarily consider life-like partially observable settings. This project, as proposed by PhD students Shuijing Liu & Peixin Chang strives to develop a reinforcement learning model for robots to navigate partially observable crowded environments (bot in simulation and on a Turtlebot). I am contributing by analyzing effectiveness of models in different scenarios & implementing additions to the simulator being used to allow for randomized initial/goal states of humans, randomizing preferred velocities and obstacle sizes, adding more policies such as Social Force, and more. These allow us to test the effectiveness of such policies in multiple situations with several variables for thoroughness.

## Challenges to Consider
* Partially observable input to robot
* Robot can be set to be unobservable to humans 
* Continuous state space
* Number of agents (humans) in state space increases complexity of calculation

## Advisors
[Shuijing Liu](https://shuijing725.github.io/), [Peixin Chang](https://sites.google.com/site/changpeixin/home?authuser=0), & [Professor Katherine Driggs-Campbell](https://krdc.web.illinois.edu/)
