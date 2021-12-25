**中文** | [EN](https://github.com/NearlyHeadlessJack/ComputerVisionPractice#readme)

# 计算机视觉课程设计
相机标定:

![building status](https://img.shields.io/badge/Ubuntu20.04%2FOpenCV4.5.3-passing-brightgreen)

![building status](https://img.shields.io/badge/Windows10%2FOpenCV4.5.3-passing-brightgreen)

![building status](https://img.shields.io/badge/Windows11%2FOpenCV4.5.3-passing-brightgreen)

## 说明
这是[东北大学信息科学与工程学院](http://www.ise.neu.edu.cn)2021年秋季学期课程《计算机视觉课程设计》的样例，这门课简单实践了计算机视觉和ROS的使用。

[东北大学计算机科学与工程学院](http://www.cse.neu.edu.cn)拥有一门2022年春季学期开设的同名课程，您可以关注[@prety-good](https://github.com/prety-good)获取更多信息。

这门课由三个分任务组成。

| 任务 | 环境需求 |
|---|---|
| **相机标定**  | OpenCV 4.5.4 <br>Ubuntu 20.04 (Windwos10/11 也可运行) |  
| **4 步相移法结构光实验** | Matlab 2020b |
| **上手实践ROS** | Ubuntu**16.04** <br>RGBD-SLAMv2 <br>PCL 1.8.0  <br>g2o(修改过的版本) <br>ROS-kinetic-full <br>& 机器人平台(课程会提供)|

## 注意事项
### 相机标定
开始之前，你需要安装OpenCV 4.0及以上版本并构建你的样例程序。你也可以通过Matlab或者Python等完成本任务。

标定程序可以通过摄像头输入也可以通过图像序列输入。你可以在**in_VID5.xml**定义这些设置，同时，这个文件也是程序运行所需要的一个参数。

最后的结果会保存在**out_camera_data.xml**中。

在编译代码之前请检查Makefile 和 CMakeLists.txt中设置是否正确。
### 上手实践ROS
因为g2o和默认PCL之间有冲突，所以不要在安装ros之后立即安装RGBD-SLAMv2。

你应该先安装经RGBD-SLAMv2作者修改后的g2o和1.8.0版本的PCL，再编辑RGBD-SLAMv2的构建设置（将默认PCL的依赖更改为PCL 1.8.0）。


