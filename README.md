# Day-3 ROS2Training : Installation setup for Tb3 (Turtlebot3)

## Clone this repo into workspace/src
https://github.com/ROBOTIS-GIT/turtlebot3_simulations

https://github.com/ROBOTIS-GIT/turtebot3

https://github.com/ROBOTIS-GIT/turtlebot3_msgs


## Run below command to install all dependent packges for tb3
rosdep install --from-paths src --ignore-src --rosdistro=humble -y

## Source gazebo environment setup
source /usr/share/gazebo/setup.bash

## Source ROS2 opt environment setup
source /opt/ros/humble/setup.bash
source install/setup.bash

## Export robot model name for simulation ( for ex: burger,waffle,waffle pi)
export TURTLEBOT3_MODEL=waffle_pi
ros2 launch turtlebot3_gazebo empty_world.launch.py
ros2 launch turtlebot3_gazebo empty_world.launch.py
