# denso_robot_ros

- Create ROS workspace

```shell
mkdir -p ~/denso_ws/src
```

- Download cobotta related packages:

```shell
cd ~/denso_ws/src

git clone https://github.com/RoboticsYY/denso_robot_ros.git

git clone https://github.com/DENSORobot/denso_cobotta_ros.git
```

- Build the workspace

```shell
sudo apt install python-catkin-tools

cd ~/denso_ws

source /opt/ros/kinetic/setup.bash

catkin build --cmake-args -DCMAKE_BUILD_TYPE=Release

source devel/setup.bash
```
