---
layout: page
title: Research
hero_height: is-small
# gallery: research_gallery
show_sidebar: false
menubar: research_menu_bar
permalink: /research/
---

# [Autonomous Driving](#autonomous-driving)

<!--  -->

{% include notification.html
message="**Structural Attention-Based Recurrent Variational Autoencoder for Highway Vehicle Anomaly Detection**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to AAMAS 2023 (full paper)</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://sites.google.com/illinois.edu/saber-vae" target="_blank"><b>[Website]</b></a>
<a href="https://arxiv.org/pdf/2301.03634.pdf" target="_blank"><b>[Paper]</b></a>
<a href="https://gitlab.engr.illinois.edu/hubris/highway-anomaly-detection" target="_blank"><b>[Code]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/lane_discretization.png" alt="Graph representation of SABeR-VAE" large_link="/img/lane_discretization.png" %}
<br>
</div>
<div class="column is-6">
<p align="justify">
In autonomous driving, detection of abnormal driving behaviors is essential to ensure the safety of vehicle controllers. Prior works in vehicle anomaly detection have shown that modeling interactions between agents improves detection accuracy, but certain abnormal behaviors where structured road information is paramount are poorly identified, such as wrong-way and off-road driving. We propose a novel unsupervised framework for highway anomaly detection which explicitly uses the structure of the environment to aid anomaly identification.
</p>
</div>
</div>

<!--  -->

{% include notification.html
message="**Towards Co-operative Congestion Mitigation**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to SAPHRI Workshop at ICRA 2022</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="/docs/saphri-icra2022_paper_8138.pdf" target="_blank"><b>[Paper]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/driving_simulator.jpg" alt="Driving simulator used to perform user studies" large_link="/img/driving_simulator.jpg" %}
</div>
<div class="column is-6">
<p align="justify">
The effects of traffic congestion are widespread and are an impedance to everyday life. Piecewise constant driving policies have shown promise in helping mitigate traffic congestion in simulation environments. We intend to use the CARLA simulator alongside the Flow framework to conduct user studies to evaluate the affect of piecewise constant driving policies.
</p>
</div>
</div>

<!--  -->

{% include notification.html
message="**Learning to Navigate Intersections with Unsupervised Driver Trait Inference**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to ICRA 2022</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://sites.google.com/illinois.edu/vae-trait-inference" target="_blank"><b>[Website]</b></a>
<a href="https://arxiv.org/pdf/2109.06783.pdf" target="_blank"><b>[Paper]</b></a>
<a href="https://github.com/Shuijing725/VAE_trait_inference" target="_blank"><b>[Code]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/rnn_vae.png" alt="Vehicle attempting to merge into an uncontrolled intersection." large_link="/img/rnn_vae.png" %}
</div>
<div class="column is-6">
<p align="justify">
Navigation through uncontrolled intersections is one of the key challenges for autonomous vehicles. Identifying the subtle differences in hidden traits of other drivers can bring significant benefits when navigating in such environments. We use a variational autoencoder with recurrent neural networks to learn a latent representation of traits without any ground truth trait labels. Then, we use this trait representation to learn a policy for an autonomous vehicle to navigate through a T-intersection with deep reinforcement learning.
</p>
</div>
</div>

# [Robotics](#robotics)

<!--  -->

{% include notification.html
message="**Intention Aware Robot Crowd Navigation with Attention-Based Interaction Graph**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Submitted to ICRA 2023</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://arxiv.org/pdf/2203.01821.pdf" target="_blank"><b>[Paper]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/crowdnav_v2.jpg" alt="Turtlebot 2i robot navigating real crowd" large_link="/img/crowdnav_v2.jpg" %}
</div>
<div class="column is-6">
<p align="justify">
We study the problem of safe and intention-aware robot navigation in dense and interactive crowds. Most previous reinforcement learning (RL) based methods fail to consider different types of interactions among all agents or ignore the intentions of people, which results in performance degradation. In this paper, we propose a novel recurrent graph neural network with attention mechanisms to capture heterogeneous interactions among agents through space and time.
</p>
</div>
</div>

<!--  -->

{% include notification.html
message="**Decentralized Structural-RNN for Robot Crowd Navigation with Deep Reinforcement Learning**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to ICRA 2022</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://sites.google.com/illinois.edu/crowdnav-dsrnn" target="_blank"><b>[Website]</b></a>
<a href="https://arxiv.org/pdf/2011.04820.pdf" target="_blank"><b>[Paper]</b></a>
<a href="https://github.com/Shuijing725/CrowdNav_DSRNN" target="_blank"><b>[Code]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/crowdnav_v1.jpg" alt="Example image" large_link="/img/crowdnav_v1.jpg" %}
</div>
<div class="column is-6">
<p align="justify">
Safe and efficient navigation through human crowds is an essential capability for mobile robots. Previous work on robot crowd navigation assumes that the dynamics of all agents are known and well-defined. In addition, the performance of previous methods deteriorates in partially observable environments and environments with dense crowds. To tackle these problems, we propose a novel network that reasons about spatial and temporal relationships for robot decision making in crowd navigation.
</p>
</div>
</div>

# [Machine Learning](#machine-learning)

<!--  -->

{% include notification.html
message="**Hierarchical Self-Imitation Learning in Single-Agent Sparse Reward Environments**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Undergraduate Thesis in IDEALS</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="/docs/SP21-ECE499-Thesis-Chakraborty, Neeloy.pdf" target="_blank"><b>[Paper]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/hac_rl.png" alt="Example image" large_link="/img/hac_rl.png" %}
</div>
<div class="column is-6">
<p align="justify">
Reinforcement learning problems with sparse and delayed rewards are challenging to solve because the algorithms explore environments to gain experience from high performing rollouts. Classical methods of encouraging exploration during training such as epsilon-greedy and noisebased exploration are not adequate on their own to explore large state spaces. This thesis presents a single agent reinforcement learning algorithm that combines the effects of SIL and HL – Generative Adversarial Self Imitation Learning + Hierarchical Actor-Critic (GASIL+HAC).
</p>
</div>
</div>

# [Computer Vision](#computer-vision)

<!--  -->

{% include notification.html
message="**World in Motion: Geometry-based Video Prediction with Visual Odometry Prediction and View Synthesis**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/world_in_motion.png" alt="Example image" large_link="/img/world_in_motion.png" %}
</div>
<div class="column is-6">
<p align="justify">
Video prediction has a wide range of applications in planning and control for robotics. More recent works have adopted stochastic models to generate sharper future frames. However, most methods do not account for camera motion and perform poorly in scenarios with moving cameras when they are deployed on autonomous vehicles and mobile robots. We propose a geometry-based prediction framework named World in Motion.
</p>
</div>
</div>
