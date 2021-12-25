[中文](https://github.com/NearlyHeadlessJack/ComputerVisionPractice/blob/main/README_ZH_CN.MD) | **EN**

# ComputerVisionPractice

## Overview
This is the complete sample of ComputerVisionPractice which is an undergraduate practice course of [NEU-ISE](http://www.ise.neu.edu.cn) on ComputerVision & ROS.(2021-Fall) 

There is another course with an identical name in [NEU-CSE](http://www.cse.neu.edu.cn) on 2022-Spring, you guys can follow [@prety-good](https://github.com/prety-good) for more information.


The course consists of 3 tasks.<br>

| Task | Requirement |
|---|---|
| **Camera Calibration**  | OpenCV 4.5.4 <br>Ubuntu 20.04 (Windwos10/11 is also available) |  
| **Phase Measurement Profilometry** | Matlab 2020b |
| **First Practice on ROS** | Ubuntu**16.04** <br>RGBD-SLAMv2 <br>PCL 1.8.0  <br>g2o(fixed) <br>ROS-kinetic-full <br>& robot platform(provided by course)|

## Notice
### Camera Calibration
To start with, you need install OpenCV 4.0+ on your PC and build the sample program. You can also acccomplish this task with Matlab or Python, etc.

The program can run in camera mode or photo sequence mode. You can decide it on **in_VID5.xml**, which the program needs when running. 

The final result will be written on **out_camera_data.xml**.

Make sure you have the right settings on Makefile & CMakeLists.txt.

### First Practice on ROS
Due to conflicts between g2o and default PCL, DO NOT install RGBD-SLAMv2 immediately after installing ROS-kinetic.

You need install g2o(special verison) and PCL 1.8.0  at first, then edit the build configuration of RGBD-SLAMv2 (replace default PCL by PCL 1.8.0).
