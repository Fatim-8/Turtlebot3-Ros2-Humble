# Turtlebot3-Ros2-Humble

This repository relates to launching and running the navigation system of the TurtleBot3 in the Gazebo simulation environment. The goal is to familiarize the user with the basic concepts of navigation and mapping using the TurtleBot3, including how to run Gazebo with the TurtleBot3 Waffle model, load the necessary ROS 2 navigation and mapping packages, launch the navigation program that controls the robot's movement and plans its path based on a pre-loaded virtual map. This allows the user to interact with the TurtleBot3 and experience its navigation and mapping capabilities in a simulated environment before moving to real-world environments.
 ## *Ensure that all necessary dependences are installed

 -Install packages
 ```
sudo apt install ros-humble-navigation2 ros-humble-nav2-bringup ros-humble-turtlebot3*
```
# 1-now Run TurtleBot3 World in Gazeboo .

1.1-export the turtlebot model
```
export TURTLEBOT3_MODEL=waffle
```
1.2-Source gazebo workspace
```
source /usr/share/gazebo/setup.bash
```
1.3-Run the turtlebot3 'waffle world'
```
ros2 launch turtlebot3_gazebo turtlebot3_world.launch.py
```
The Gazebo simulation with the TurtleBot3 world will run as follows:
