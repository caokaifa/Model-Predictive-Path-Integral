1.一个压缩文件为仿真环境，一个压缩文件为MPPI算法
2.仿真环境为ubuntu18.04+melodic，仿真为差速底盘
3.建立ROS工程与src文件夹，把这两个文件放入编译
4.启动仿真环境
roslaunch roborts_bringup roborts_stage.launch
然后启动决策模块：
rosrun roborts_decision behavior_test_node
选择模式6进入点到点导航
5.然后启动MPPI算法模块
启动MPPI前输入的转换模块
 roslaunch reference_costmap_generator reference_costmap_generator.launch
 启动MPPI算法
 
 roslaunch mppi_3d mppi_3d_a.launch
file:///home/smart/Pictures/Screenshot%20from%202024-12-18%2010-35-58%20-%201.png![image](https://github.com/user-attachments/assets/ec66d1ac-f56a-49c4-9f26-9d0ad43bed5d)
