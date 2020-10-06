---
layout: default
---

# Volunteering at UBC VCR (Verification, Control, Robotics)

May 2020 to Present

## Summary
Under [Prof. Ian Mitchell](https://www.cs.ubc.ca/~mitchell/)'s supervision, I have been working on a project aimed for building an interface between ROS and [AI Habitat](https://aihabitat.org/). 
<br><br>

## What is AI Habitat and what is ROS? Why together?
AI Habitat is a reinforcement learning framework used for training and evaluating embodied agents on various tasks, such as visual navigation and language navigation. The framework consists of two parts: 1) Habitat Lab, an API for task definition, training, testing, and 2) Habitat Sim, a simulator. 

ROS is a robotics middleware which allows us to develop robotics software on top of. For example, we can construct a SLAM-based agent and simulate it within the Gazebo simulator under the ROS framework.

AI Habitat provides novel methods for defining tasks and RL-based agents, and a photorealistic simulator. ROS on the other hand is where most traditional agents or software in general run within. So we aim to bridge the gap between the frameworks. 

## My roles in the project
Built upon existing work by [Bruce Cui](https://ca.linkedin.com/in/brucecui97), I'm continuing the development of the ROSxHabitat Interface. Specifically, for the interface, we want it to be able to
* allow communication between agents trained under Habitat to use ROS-based simulators;
* allow communication between agents from ROS packages work under Habitat Sim.

Here is an architectural diagram of the interface:

![](ros_x_hab_interface_arch.PNG)
*Architecture of ROSxHabitat Interface. Grabbed from my presentation slides for VCR*

Recently, Habitat Sim incorporated the Bullet engine to simulate physics effects. We are investigating how this change would affect the simulation of Habitat-trained agents, while in the mean time accomodating the change in our interface.

