# nav_slam
slam建图
cd 包名
source devel/setup.bash

roslaunch urdf02_gazebo de03_env.launch

source ./devel/setup.bash
roslaunch nav_demo nav01_slam.launch

另开终端
rosrun teleop_twist_keyboard teleop_twist_keyboard.py

保存地图
source ./devel/setup.bash
roslaunch nav_demo de02_map_save.launch

AMCL使用
source ./devel/setup.bash
roslaunch urdf02_gazebo de03_env.launch
roslaunch nav_demo test_amcl.launch

base_move使用
source ./devel/setup.bash
roslaunch urdf02_gazebo de03_env.launch

功能包中另开终端
source ./devel/setup.bash
roslaunch nav_demo nav06_test.launch

最后集成,也是用于自动导航的启动
source ./devel/setup.bash
roslaunch nav_demo nav07_slam_auto.launch
