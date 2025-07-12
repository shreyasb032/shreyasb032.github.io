---
title: "Trustworthy Human-AGV Interaction"
excerpt: "In this project, we try to generate trustworthy behaviors for Automated Guided Vehicles (AGVs) while interacting with human workers in shared workspaces in manufacturing plants.<br/><img src='/images/fam-paper-cover-image.png'> <br/>As a first step, we modeled worker motion as a Finite Automaton Model (FAM) with 6 intuitive states and transition functions that could be set up easily once we get the plan of the manufacturing plant. As a second step, we have added predictive modeling to the basic FAM model..."
collection: projects
---

# Trustworthy Human-AGV Interaction

In this project, we try to generate trustworthy behaviors for Automated Guided Vehicles (AGVs) while interacting with human workers in shared workspaces in manufacturing plants. As a first step, we modeled worker motion as a Finite Automaton Model (FAM) with 6 intuitive states and transition functions that could be set up easily once we get the plan of the manufacturing plant. The image below shows an illustration of how these states work as a worker moves around in the manufacturing plant.

<img src='/images/fam-paper-cover-image.png'>

We developed a Virtual Reality version of a real-life manufacturing plant used by Boeing using Unreal Engine. The images below show some screenshots of the VR environment. 

<img src='/images/VR-testbed-screenshots.png'>

The participants in our study are able to freely walk around in the environment using the Meta Quest Pro headset and the KAT Walk C2 Omnidirectional treadmill. They are also able to interact with objects in the environment using the hand-held controllers. These equipment are shown in images below.

<img src='/images/VR-equipment.png'>

This project has led to 1 peer-reviewed conference proceedings.

We are currently working on developing a Temporal Fusion Transformer (TFT) based trajectory prediction model that leverages the state-of-the-art diffusion models to generate future positions of the workers in the next 4 seconds. Using these predicted positions, the AGVs can then modify their own behavior (e.g. slow down, indicate it's intent using eHMIs, move around, etc.). At the current stage of the project, our model only predicts the future trajectory of one agent. We are currently working towards extending this to multi-agent scenarios with explicit inter-agent interaction modeling. We will pre-train this model using open-source datasets and then fine-tune using some simulated data. Towards that, we will also be developing a multi-agent simulator in Unreal Engine using behavior trees.


### Selected Publications

- [Identifying Worker Motion Through a Manufacturing Plant: A Finite Automaton Model](https://ieeexplore.ieee.org/abstract/document/10731360), *IEEE International Conference on Human-Robot Interactive Communication (RO-MAN)*, 2025
