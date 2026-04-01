# Urdf_my-car-robot-arm
3.27第四周实验课程，urdf的编写和Gazebo仿真的运用

# 编译与运行 1. **编译工作空间** 进入工作空间目录并进行编译：
cd ~/wx_ros_class_ws 
catkin_make 
source devel/setup.bash

# 启动 Gazebo 仿真环境：
roslaunch wx_robot_description gazebo.launch

# 自己的机器人 urdf启动和xarco启动
roslaunch wx_robot_description display.launch

roslaunch wx_robot_description display_xarco.launch

#启动键盘控制指令
rosrun teleop_twist_keyboard teleop_twist_keyboard.py


# 机械臂启动（在zx_robot_description功能包内调用）
roslaunch zx_robot_description w2a_arm.launch
#rqt控制关节
rosrun rqt_joint_trajectory_controller rqt_joint_trajectory_controller

