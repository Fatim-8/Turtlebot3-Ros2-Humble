# Turtlebot3-Ros2-Humble

This repository relates to launching and running the navigation system of the TurtleBot3 in the Gazebo simulation environment. The goal is to familiarize the user with the basic concepts of navigation and mapping using the TurtleBot3, including how to run Gazebo with the TurtleBot3 Waffle model, load the necessary ROS 2 navigation and mapping packages, launch the navigation program that controls the robot's movement and plans its path based on a pre-loaded virtual map. This allows the user to interact with the TurtleBot3 and experience its navigation and mapping capabilities in a simulated environment before moving to real-world environments.
 ## *Ensure that all necessary dependences are installed

 -Install packages
 ```
sudo apt install ros-humble-navigation2 ros-humble-nav2-bringup ros-humble-turtlebot3*
```
# 1-now Run TurtleBot3 World in Gazebo .

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
(<img width="535" alt="image" src="https://github.com/user-attachments/assets/3ac14048-9bf4-410d-9ea1-fb99912ea666">

# 2-Now we can control the Turtlebot3 robot using the keyboard, open another terminal
2.1-Export the required variable
```
export TURTLEBOT3_MODEL=waffle
```
2.2-Run the teleop_key node
```
ros2 run turtlebot3_teleop teleop_keyboard
```
# 3- To Create and Save a map using "SLAM"
Run this command to save the map:
```
ros2 run nav2_map_server map_saver_cli -f ~/filename
```


