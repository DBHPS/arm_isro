```source /opt/ros/humble/setup.bash && colcon build --symlink-install && source install/setup.bash && source install/local_setup.bash```

`ros2 launch arm_description gazebo.launch.py`
`ros2 launch isro_arm_controller controller.launch.py`
`ros2 launch arm_description display.launch.py`
