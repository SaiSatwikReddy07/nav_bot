# NavBot
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#Description">Description</a></li>
    <li><a href="#Pre-requisites">Pre-requisites</a></li>
    <li><a href="#Usage">Usage</a></li>
    <li><a href="#Repository-Tree">Repository Tree</a></li>
    <li><a href="#Simulation-Visuals">Simulation Visuals</a></li>
    <li><a href="#Demonstration-Video">Demonstration Video</a></li>
    <li><a href="#Real-Life-Applications">Real Life Applications</a></li>
  </ol>
</details>

## Description
----
Our project develops a simulated environment for a 4-wheeled robot with advanced functionalities like object sensing, path planning, and sign board classification. It combines ROS2 and Gazebo for a realistic simulation. Sensors such as cameras, and lidar enable object sensing, facilitating safe navigation. Path planning allows the robot to navigate optimal paths and adapt to changes. Signboard classification using OpenCV enhances decision-making and adherence to traffic rules.
![Screenshot from 2023-06-27 17-22-50](https://github.com/SaiSatwikReddy07/NavBot/assets/109800395/690771f3-1398-4fd1-999d-422be7bbfb08)

## Pre-requisites
----
* Ubuntu 22.04 
* ROS2 - Humble
* Python 3
* Opencv 4
* Yolov5
* Gazebo 11.10.2
* rviz2
## Usage
----
<code>
ros2 launch nav_bot launch_sim.launch.py world:=navbot.world
</code> 

## Repository Tree
----
![image](https://github.com/SaiSatwikReddy07/NavBot/assets/109800395/6458b364-5a7d-4526-b216-192e8825bd88)

## Simulation Visuals
----

## Demonstration Video
----

## Real Life Application
----
* Autonomous Driving Cars
