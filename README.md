<!--
 * @Descripttion: 
 * @version: 
 * @Author: LitoNeo
 * @Date: 2020-01-13 13:26:13
 * @LastEditors  : LitoNeo
 * @LastEditTime : 2020-01-13 14:10:25
 -->
# SmartCar-Tools
Tools for self-driving car

## 写在前面
1. 每个单独的模块都有自己的使用说明,参考模块自身的`README.md`
2. 关于环境配置问题,我正在制作Docker镜像

## How to Build
This repo depends on QT-5.9 and ROS1.0, be sure it is correctly installed on your pc.
I tested it on `Ubuntu1604`.

1. `mkdir -p catkin_ws/src && cd catkin_ws/src`
2. `git clone https://github.com/LitoNeo/SmartCar-Tools.git`
3. `cd .. && catkin_make`

## map_tools
> Tools used to process map data.(especially for pcd files)
1. **trajectory_generator**
A qt-based tools used to define and extract drivable trajectory.
Currently it only extracts drivable trajectories, that is, a minimum subset of high-precision maps. But it is flexible to extend.

2. **grid_map_generator**
A qt-based tools to downsample and mesh the big pcd maps to small one.   
For more details, refer [here](https://zhuanlan.zhihu.com/p/77745476)


## driver
> useful driver for self-driving car
