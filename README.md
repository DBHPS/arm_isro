Demonstration:- https://youtu.be/uZn7K_7etnw?si=P6nMppIMYyfs3wXd


BOM:-  https://docs.google.com/spreadsheets/d/1sL7dMYFJnx55CJGOrdYcx4CreSIZwntF3HYR8WQRc48/edit?usp=sharing


install ros2 humble on ubunutu 22 from https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debs.html

Git clone the project


##
        sudo apt-get update && sudo apt-get dist-upgrade && sudo apt install python3-colcon-common-extensions && sudo apt install ros-humble-xacro && sudo apt install ros-humble-joint-state-publisher-gui && sudo apt install ros-humble-gazebo-ros-pkgs && sudo apt install ros-humble-ros2-control ros-humble-ros2-controllers && sudo apt-get install ros-humble-moveit-ros-move-group && sudo apt install ros-humble-gazebo-ros2-control




# Go inside arm_ws and create 4 separate instaces of terminal 


### Sourcing ROS on each and every terminal 
##
        source /opt/ros/humble/setup.bash && colcon build --symlink-install && source install/setup.bash && source install/local_setup.bash


### Launch file for RVIZ2
##
        ros2 launch arm_description display.launch.py


### Launch file for Gazebo
##
        ros2 launch arm_description gazebo.launch.py


### Launch file for ros2 control
##
        ros2 launch isro_arm_controller controller.launch.py



### Launch file for moveit and arm trajectory control
##
        ros2 launch isro_arm_moveit moveit.launch.py


### May be required
##
        sudo apt-get install ros-humble-tf-transformations
##
        sudo pip3 install transforms3d
##
        sudo apt install ros-humble-rmw-cyclonedds-cpp
##
        sudo apt-get install ros-humble-moveit

### in bashrc
##
        export RMW_IMPLEMENTATION=rmw_cyclonedds_cpp









