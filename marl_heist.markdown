---
layout: page
title: Multi Agent Reinforcement Learning in Randomized Heist Environments
hero_height: is-small
permalink: /marl_heist/
---

## Purpose
As robots become more ingrained in our day to day tasks, it is important to consider how these agents can adapt to work with humans in a variety of environments. For my undergraduate senior research project, I propose one method of testing effectiveness of collaboration of agents in simulation via multi agent algorithms and environments. Specifically, I plan to adapt the Heist environment developed by OpenAI's Procgen project (a procedurally generated randomized single agent environment), into a multi agent environment. In this situation, agents who know little about each other from the beginning must collaborate to gather keys from a simulated maze, and reach the exit together over multiple levels. This new problem statement forces agents to communicate with one another, and during the training process, they must have high exploration capability to find keys randomly placed. If time permits, I would also like to explore how to incorporate a trust signal within agents, which may impact their actions according to the level of trust in other agents. A simplified version of this work will be integrated and demonstrate on hardware using the Turtlebot platform.  
  
Details about the Procgen Heist environment I will be modifying can be found [here](https://github.com/openai/procgen).

## Challenges to Consider
* Encouraging collaboration among agents during training
* Sparse rewards require high exploration
* Number of timesteps to end state during training may be large
* Consider filtering input observation space to agents to simplify complexity
* Continuous state space

## Advisor
[Professor Katherine Driggs-Campbell](https://krdc.web.illinois.edu/)
