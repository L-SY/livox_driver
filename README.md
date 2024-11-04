#### livox_driver

> It is convenient to use Livox mid360 in the ROS1 noetic version under Ubuntu 20.04

`livox_laser_simulation`  is change from https://github.com/fratopa/Mid360_simulation_plugin, unnecessary test files have been removed from the original project, and xacro files have been added for easy addition in urdf.

`livox_ros_driver2`  is change from https://github.com/Livox-SDK/livox_ros_driver2, Adaptation to livox-SDK2 and changes ros1 compilation to use catkin build instead of catkin_make.


#### Build

```bash
git submodule update --init
cd /livox_driver/Livox-SDK2
mkdir build && cd build
cmake ..
make install
cd ../..
catkin build
```
