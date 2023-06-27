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
1. Run the following code after changing the directory to the path where the world file is located. <br/>
<code>ros2 launch nav_bot launch_sim.launch.py world:=navbot.world</code> <br/>
2. Open a new terminal in the workspace directory, and run the following code: <br/>
<code>ros2 launch nav_bot online_async_launch.py params_file:=./src/nav_bot/config/mapper_params_online_async.yaml use_sim_time:=true</code> <br/>
3. Open a new terminal in the workspace directory again, and run the following code: <br/>
<code>ros2 launch nav2_bringup navigation_launch.py use_sim_time:=true</code> <br/>
4. Open a new terminal in /yolobot_recognition/scripts/, and run the following code: <br/>
<code>python3 ros_recognition_yolo.py</code> <br/>
5. The locations of serialized files nav_bot.posegraph and nav_bot.data should be provided inside the variable 'map_file_name' in the file  'mappers_params_online_async.yaml'.
  
## Repository Tree
----
![image](https://github.com/SaiSatwikReddy07/NavBot/assets/109800395/6458b364-5a7d-4526-b216-192e8825bd88)

## Simulation Visuals
----
* Sign Board Classification <br/>
![Screenshot from 2023-06-27 17-34-20](https://github.com/SaiSatwikReddy07/NavBot/assets/109800395/4694f3be-00f3-4778-8781-c7b1854d1128) <br/>
* rviz2 <br/>
![Screenshot from 2023-06-27 17-23-54](https://github.com/SaiSatwikReddy07/NavBot/assets/109800395/5eabf78d-1cca-46d6-a0ee-498f4d41a81e) <br/>
* World <br/>
![Screenshot from 2023-06-27 17-22-50](https://github.com/SaiSatwikReddy07/NavBot/assets/109800395/97ed6acb-5ca1-4b96-8681-a9060e915ad5) <br/>
* Stop Sign <br/>
![Screenshot from 2023-06-27 17-23-21](https://github.com/SaiSatwikReddy07/NavBot/assets/109800395/8c81a4a0-433b-44e7-9ccf-40777044b03c) <br/>

## Demonstration Video
----
* Click the below picture for the complete working video on youtube <br/>
[![YouTube Video](http://img.youtube.com/vi/UnKrqkgXtco/0.jpg)](https://youtu.be/UnKrqkgXtco)
## Real-Life Application
----
* Autonomous Driving Cars
