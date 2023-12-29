---
layout: page
title: Real Time Path Planning and Obstacle Avoidance of Quadcopter in 3D Space
description: Autonomous drone to avoid static obstacles
img: obstacle_avoidance_drone(1).gif
importance: 1
category: work
related_publications: einstein1956investigations, einstein1950meaning
---

# Real Time Path Planning and Obstacle Avoidance in 3D Space

In these past few years, Unmanned Aerial Vehicles (UAVs) have undergone tremendous development and acquired fast-growing popularity worldwide. UAVs applications are not restricted to military and defence: the civilian UAVs market covers a wide scope of domains, for example, traffic surveillance, disaster management, infrastructure inspection, law enforcement, and vegetation monitoring etc. With such vast applications which require split second decisions to be made in real time it is important that the UAV flies without any human intervention and relies on the onboard sensors and computers to work. In UAV flight, obstacle avoidance thus becomes important and path planning must be taken care of in real time to avoid static as well as dynamic obstacles.

How the code works 
1. The drone detects the obstacles position using a stereo camera
2. The obstacles position is used to generate a local map
3. An obstacle free path is found around the obstacle avoiding it succesfully in real time

The path generation takes place using RRT in less than 1 second.

## Work Pending 
1. Convert the code to CPP for faster detection and path generation
2. Rigourous testing on hardware to improve the pipeline
3. Use voxel grids to reduce the computation load.


In the video, the drone detects the obstacle visualized by the point cloud(top left)
It generates a new path around the obstacle seen at the bottom left

## Tools used
1. Python
2. PX4 with Mavros and ROS
3. Gazebo for visualization
4. Point cloud library
