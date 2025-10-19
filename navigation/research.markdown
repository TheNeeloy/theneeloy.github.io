---
layout: page
title: Research
hero_height: is-small
show_sidebar: false
menubar: research_menu_bar
permalink: /research/
---

# [Foundation Model Evaluation](#fm-eval)

<!--  -->

{% include notification.html
message="**Adaptive Stress Testing Black-Box LLM Planners**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>arXiv 2025 Pre-Print</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://arxiv.org/abs/2505.05665" target="_blank"><b>[Paper]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/ast_block.png" alt="Block diagram of adaptive stress testing framework" large_link="/img/ast_block.png" %}
<br>
</div>
<div class="column is-6">
<p align="justify">
Large language models (LLMs) have recently demonstrated success in generalizing across decision-making tasks including planning, control, and prediction, but their tendency to hallucinate unsafe and undesired outputs poses risks. We argue that detecting such failures is necessary, especially in safety-critical scenarios. We propose a novel method for efficiently searching the space of prompt perturbations using adaptive stress testing (AST) with Monte-Carlo tree search (MCTS). Our AST formulation enables discovery of scenarios and prompts that cause language models to act with high uncertainty or even crash.
</p>
</div>
</div>

<!--  -->

{% include notification.html
message="**Hallucination Detection in Foundation Models for Decision-Making: A Flexible Definition and Review of the State of the Art**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to ACM Computing Surveys 2025</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://arxiv.org/abs/2403.16527" target="_blank"><b>[Paper]</b></a>
<a href="https://doi.org/10.1145/3716846" target="_blank"><b>[DOI]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/hallucination_example.png" alt="Block diagram of examples of hallucinations faced by an LVLM planner in deployment" large_link="/img/hallucination_example.png" %}
<br>
</div>
<div class="column is-6">
<p align="justify">
While researchers have shown promising results in deploying foundation models to decision-making tasks, these models are known to hallucinate and generate decisions that may sound reasonable, but are in fact poor. We argue there is a need to step back and simultaneously design systems that can quantify the certainty of a model's decision, and detect when it may be hallucinating. In this work, we discuss the current use cases of foundation models for decision-making tasks, provide a general definition for hallucinations with examples, discuss existing approaches to hallucination detection and mitigation with a focus on decision problems, present guidelines, and explore areas for further research in this exciting field.
</p>
</div>
</div>

# [Field Robotics](#field-robots)

<!--  -->

{% include notification.html
message="**Towards Real-Time Generation of Delay-Compensated Video Feeds for Outdoor Mobile Robot Teleoperation**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to ICRA 2025</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://sites.google.com/illinois.edu/comp-teleop" target="_blank"><b>[Website]</b></a>
<a href="https://arxiv.org/abs/2409.09921" target="_blank"><b>[Paper]</b></a>
<a href="https://doi.org/10.1109/ICRA55743.2025.11128424" target="_blank"><b>[DOI]</b></a>
<a href="https://github.com/thehcalab-uiuc/DeCompTeleop" target="_blank"><b>[Code]</b></a>
<a href="https://uofi.box.com/s/arc2wswqfk0ksld6zovexlj3eayiv20o" target="_blank"><b>[Dataset]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/teleop_cover.png" alt="The TerraSentia+ robot in dense growth and an example of a remote teleoperation setup" large_link="/img/teleop_cover.png" %}
<br>
</div>
<div class="column is-6">
<p align="justify">
We propose a modular learning-based vision pipeline to generate delay-compensated images in real-time for supervisors. Our extensive offline evaluations demonstrate that our method generates more accurate images compared to state-of-the-art approaches in our setting. Additionally, ours is one of the few works to evaluate a delay-compensation method in outdoor field environments with complex terrain on data from a real robot in real-time.
</p>
</div>
</div>

# [Autonomous Driving](#autonomous-driving)

<!--  -->

{% include notification.html
message="**An Expert Ensemble for Detecting Anomalous Scenes, Interactions, and Behaviors in Autonomous Driving**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to Sage IJRR 2024</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://arxiv.org/abs/2502.16389" target="_blank"><b>[Paper]</b></a>
<a href="https://doi.org/10.1177/02783649241297998" target="_blank"><b>[DOI]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/xen_beh.png" alt="Qualitative evaluations of the behavior expert from Xen in example scenarios" large_link="/img/xen_beh.png" %}
<br>
</div>
<div class="column is-6">
<p align="justify">
The ability to detect anomalous situations outside of the operational design domain is a key component in self-driving cars, enabling us to mitigate the impact of abnormal ego behaviors and to realize trustworthy driving systems. On-road anomaly detection in egocentric videos remains a challenging problem due to the difficulties introduced by complex and interactive scenarios. We conduct a holistic analysis of common on-road anomaly patterns, from which we propose three unsupervised anomaly detection experts: a scene expert that focuses on frame-level appearances to detect abnormal scenes and unexpected scene motions; an interaction expert that models normal relative motions between two road participants and raises alarms whenever anomalous interactions emerge; and a behavior expert which monitors abnormal behaviors of individual objects by future trajectory prediction.
</p>
</div>
</div>

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
<a href="https://arxiv.org/abs/2301.03634" target="_blank"><b>[Paper]</b></a>
<a href="https://dl.acm.org/doi/10.5555/3545946.3598754" target="_blank"><b>[DOI]</b></a>
<a href="https://github.com/thehcalab-uiuc/Highway-Anomaly-Detection" target="_blank"><b>[Code]</b></a>
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
<a href="https://sites.google.com/view/vae-trait-inference/home" target="_blank"><b>[Website]</b></a>
<a href="https://arxiv.org/abs/2109.06783" target="_blank"><b>[Paper]</b></a>
<a href="https://doi.org/10.1109/ICRA46639.2022.9811635" target="_blank"><b>[DOI]</b></a>
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

# [Instruction-Following Agents](#instruction-following)

<!--  -->

{% include notification.html
message="**A Data-Efficient Visual-Audio Representation with Intuitive Fine-tuning for Voice-Controlled Robots**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to CoRL 2023</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://sites.google.com/site/changpeixin/home/Research/a-data-efficient-visual-audio-representation-with-intuitive-fine-tuning?authuser=0" target="_blank"><b>[Website]</b></a>
<a href="https://arxiv.org/abs/2301.09749" target="_blank"><b>[Paper]</b></a>
<a href="https://proceedings.mlr.press/v229/chang23a.html" target="_blank"><b>[DOI]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/kuka_rep_small.png" alt="Visualizations of the VAR embedding space" large_link="/img/kuka_rep_small.png" %}
<br>
</div>
<div class="column is-6">
<p align="justify">
A command-following robot that serves people in everyday life must continually improve itself in deployment domains with minimal help from its end users, instead of engineers. Previous methods are either difficult to continuously improve after the deployment or require a large number of new labels during fine-tuning. Motivated by (self-)supervised contrastive learning, we propose a novel representation that generates an intrinsic reward function for command-following robot tasks by associating images with sound commands. After the robot is deployed in a new domain, the representation can be updated intuitively and data-efficiently by non-experts without any hand-crafted reward functions.
</p>
</div>
</div>

<!--  -->

{% include notification.html
message="**BEAST: Building an Embodied Action-Prediction System with Trajectory Data**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Competed in the 2023 Amazon SimBot Competition</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://www.amazon.science/alexa-prize/teams/kingfisher-2022" target="_blank"><b>[Team Kingfisher]</b></a>
<a href="https://www.amazon.science/alexa-prize/proceedings/beast-building-an-embodied-action-prediction-system-with-trajectory-data" target="_blank"><b>[Paper]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-3by4" link="/img/simbot_flow.png" alt="Block diagram of the BEAST architecture" large_link="/img/simbot_flow.png" %}
<br>
</div>
<div class="column is-6">
<p align="justify">
We introduce our system BEAST (Building an Embodied Action-prediction System with Trajectory data) for interactive instruction-following within the Alexa Arena Platform. Our system leverages the abstraction of navigation provided by the Arena to decouple the language and vision predictions. This allows for greater simplicity within the system, and for rapid augmentation of the trajectory data-set and training for our text-only action prediction model. By creating a framework with a focus towards user experience our system is more robust to errors in predictions, and informative to the user.
</p>
</div>
</div>

# [Robot Crowd Navigation](#crowdnav)

<!--  -->

{% include notification.html
message="**HEIGHT: Heterogeneous Interaction Graph Transformer for Robot Navigation in Crowded and Constrained Environments**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to IEEE T-ASE 2025</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://sites.google.com/view/crowdnav-height/home" target="_blank"><b>[Website]</b></a>
<a href="https://arxiv.org/abs/2411.12150" target="_blank"><b>[Paper]</b></a>
<a href="https://github.com/Shuijing725/CrowdNav_HEIGHT" target="_blank"><b>[Code]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/crowdnav_v3.png" alt="Turtlebot 2i robot navigating real crowd" large_link="/img/crowdnav_v3.png" %}
</div>
<div class="column is-6">
<p align="justify">
We study the problem of robot navigation in dense and interactive crowds with environmental constraints such as corridors and furniture. Previous methods fail to consider all types of interactions among agents and obstacles, leading to unsafe and inefficient robot paths. In this article, we leverage a graph-based representation of crowded and constrained scenarios and propose a structured framework to learn robot navigation policies with deep reinforcement learning.
</p>
</div>
</div>

<!--  -->

{% include notification.html
message="**Intention Aware Robot Crowd Navigation with Attention-Based Interaction Graph**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to ICRA 2023</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://sites.google.com/view/intention-aware-crowdnav/home" target="_blank"><b>[Website]</b></a>
<a href="https://arxiv.org/abs/2203.01821" target="_blank"><b>[Paper]</b></a>
<a href="https://doi.org/10.1109/ICRA48891.2023.10160660" target="_blank"><b>[DOI]</b></a>
<a href="https://github.com/Shuijing725/CrowdNav_Prediction_AttnGraph" target="_blank"><b>[Code]</b></a>
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
<b>Accepted to ICRA 2021</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://sites.google.com/view/crowdnav-ds-rnn/home" target="_blank"><b>[Website]</b></a>
<a href="https://arxiv.org/abs/2011.04820" target="_blank"><b>[Paper]</b></a>
<a href="https://doi.org/10.1109/ICRA48506.2021.9561595" target="_blank"><b>[DOI]</b></a>
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

# [Traffic Congestion Mitigation](#carp)

<!--  -->

{% include notification.html
message="**Lessons in Cooperation: A Qualitative Analysis of Driver Sentiments towards Real-Time Advisory Systems from a Driving Simulator User Study**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to IEEE ITSM 2025</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://arxiv.org/abs/2407.13775" target="_blank"><b>[Paper]</b></a>
<a href="https://doi.org/10.1109/MITS.2025.3555564" target="_blank"><b>[DOI]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-2by1" link="/img/carp_lessons.png" alt="Visual of how CARP algorithms influence driver sentiments" large_link="/img/carp_lessons.png" %}
</div>
<div class="column is-6">
<p align="justify">
Real-time Advisory (RTA) systems, such as navigational and eco-driving assistants, are becoming increasingly ubiquitous in vehicles due to their benefits for users and society. Until autonomous vehicles mature, such advisory systems will continue to expand their ability to cooperate with drivers, enabling safer and more eco-friendly driving practices while improving user experience. However, the interactions between these systems and drivers have not been studied extensively. To this end, we conduct a driving simulator study (N=16) to capture driver reactions to a Cooperative RTA system.
</p>
</div>
</div>

<!--  -->

{% include notification.html
message="**Cooperative Advisory Residual Policies for Congestion Mitigation**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to ACM JATS 2024</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://arxiv.org/abs/2407.00553" target="_blank"><b>[Paper]</b></a>
<a href="https://doi.org/10.1145/3699519" target="_blank"><b>[DOI]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-16by9" link="/img/carp.jpg" alt="Block diagram of the PeRP framework" large_link="/img/carp.jpg" %}
</div>
<div class="column is-6">
<p align="justify">
Fleets of autonomous vehicles can mitigate traffic congestion through simple actions, thus improving many socioeconomic factors such as commute time and gas costs. However, these approaches are limited in practice as they assume precise control over autonomous vehicle fleets, incur extensive installation costs for a centralized sensor ecosystem, and also fail to account for uncertainty in driver behavior. To this end, we develop a class of learned residual policies that can be used in cooperative advisory systems and only require the use of a single vehicle with a human driver. Our policies advise drivers to behave in ways that mitigate traffic congestion while accounting for diverse driver behaviors, particularly drivers' reactions to instructions, to provide an improved user experience.
</p>
</div>
</div>

<!--  -->

{% include notification.html
message="**PeRP: Personalized Residual Policies For Congestion Mitigation Through Co-operative Advisory Systems**"
icon="false"
status="is-success" %}

#### []()

<div class="columns">
<div class="column is-6">
<p align="center">
<b>Accepted to ITSC 2023</b>
</p>
</div>
<div class="column is-6">
<p align="center">
<a href="https://sites.google.com/illinois.edu/perp" target="_blank"><b>[Website]</b></a>
<a href="https://arxiv.org/abs/2308.00864" target="_blank"><b>[Paper]</b></a>
<a href="https://doi.org/10.1109/ITSC57777.2023.10422444" target="_blank"><b>[DOI]</b></a>
<a href="https://github.com/thehcalab-uiuc/PeRP" target="_blank"><b>[Code]</b></a>
</p>
</div>
</div>

<div class="columns">
<div class="column is-6">
{% include image-modal.html ratio="is-2by1" link="/img/perp.png" alt="Visualization of how PeRP mitigates traffic by providing personalized advice to drivers" large_link="/img/perp.png" %}
</div>
<div class="column is-6">
<p align="justify">
Intelligent driving systems can be used to mitigate congestion through simple actions, thus improving many socioeconomic factors such as commute time and gas costs. However, these systems assume precise control over autonomous vehicle fleets, and are hence limited in practice as they fail to account for uncertainty in human behavior. Piecewise Constant (PC) Policies address these issues by structurally modeling the likeness of human driving to reduce traffic congestion in dense scenarios to provide action advice to be followed by human drivers. However, PC policies assume that all drivers behave similarly. To this end, we develop a co-operative advisory system based on PC policies with a novel driver trait conditioned Personalized Residual Policy, PeRP. PeRP advises drivers to behave in ways that mitigate traffic congestion.
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
<a href="https://arxiv.org/abs/2302.09140" target="_blank"><b>[Paper]</b></a>
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
{% include image-modal.html ratio="is-1by1" link="/img/hac_rl.png" alt="Example image" large_link="/img/hac_rl.png" %}
</div>
<div class="column is-6">
<p align="justify">
Reinforcement learning problems with sparse and delayed rewards are challenging to solve because the algorithms explore environments to gain experience from high performing rollouts. Classical methods of encouraging exploration during training such as epsilon-greedy and noisebased exploration are not adequate on their own to explore large state spaces. This thesis presents a single agent reinforcement learning algorithm that combines the effects of SIL and HL – Generative Adversarial Self Imitation Learning + Hierarchical Actor-Critic (GASIL+HAC).
</p>
</div>
</div>
