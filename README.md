# ROS Wrapper for Intel&reg; RealSense&trade; Devices - DIME
This repository contains a modified version of the [Intel's realsense-ros] repository, which is part of the official implementation of [DIME](https://arxiv.org/abs/2203.13251). The base repo containing all the information can be found at [DIME - Models](https://github.com/NYU-robot-learning/DIME-Models).

## Installation Instructions
You need to install the [`librealsense`](https://github.com/IntelRealSense/librealsense#installation-guide) API provided by Intel followed by [ROS Noetic](http://wiki.ros.org/noetic/Installation/Ubuntu) and then make the binaries using `catkin_make` command.

## Running the ROSLaunch file
To run the ROSLaunch file, use the following command:
```
source <base-camera-dir>/devel/setup.bash
roslaunch realsense2_camera rs_camera.launch camera:=cam_<camera_number> serial_no:=<camera_serial_number>
``` 

## Citation 
If you use this repo in your research, please consider citing the paper as follows:
```
@article{arunachalam2022dime,
  title={Dexterous Imitation Made Easy: A Learning-Based Framework for Efficient Dexterous Manipulation},
  author={Sridhar Pandian Arunachalam and Sneha Silwal and Ben Evans and Lerrel Pinto},
  journal={arXiv preprint arXiv:2203.13251},
  year={2022}
}
```