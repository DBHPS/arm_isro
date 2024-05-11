### Sourcing ROS

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


