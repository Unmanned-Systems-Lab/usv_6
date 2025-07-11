## 1、编译

进入usv_6文件夹，直接catkin_make

## 2、启动

`roslaunch bringup bringup_simulation.launch`

新开一个终端，运行rqt，添加plugins中topics的message publisher

选择/cmd_vel，把频率改成10hz，然后点击加号发布这个话题，最后把/cmd_vel话题中linear的x速度改为1.0，就可以看到6个无人艇都在往前移动了

## 3、安装依赖包
如果发现只有点云没有占据栅格地图，就把所需的ros包安装完整：

`sudo apt install ros-noetic-hector*`

`sudo apt install ros-noetic-velodyne*`

`sudo apt install ros-noetic-map-server`

`sudo apt install ros-noetic-robot-localization`
