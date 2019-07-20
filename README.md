# awesome-ros-mobile-robot  [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/shannon112/awesome-ros-mobile-robot)  
This repository provides some useful resources and informations about **autonomous mobile robots (AMR)** research based on **ROS**. It would not contain high level application, but focus on basic function of mobile robots(and more at **odometry**). (including both **Chinese** and **English** materials)  

## contents:  
* [0.Robotics](README.md#0_robotics)
* [1.ROS](README.md#1_ros)
* [2.Robot platform](README.md#2_robot_platform)
* [3.Robot sensor](README.md#3_robot_sensor)
* [4.Odometry](README.md#4_odometry)
* [5.SLAM](README.md#5_slam)
* [6.Localization](README.md#6_localization)
* [7.MAP](README.md#7_map)
* [8.Navigation (move_base)](README.md#8_navigation_movebase)
* [9.Navigation (advanced)](README.md#9_navigation_advanced)
* [10.Others (Non-tech)](README.md#10_others_non_tech_part)
  * (1)Famous robotics company  
  * (2)Famous robotics conference&journal  
  * (3)Famous robotics competition in Taiwan  
  * (4)Famous ros organizations & activities  

## 0_Robotics
Books:
```js
"Multiple View Geometry in Computer Vision", Richard Hartley, Andrew Zisserman
"Probabilistic Robotics", Sebastian Thrun 
"Introduction to Linear Algebra", Five Edition, Gilbert Strang
"視覺 SLAM 十四講：從理論到實踐", 高翔
```
Courses:
```js
"Robot Mapping" {Universität of Freiburg} Cyrill Stachniss: http://ais.informatik.uni-freiburg.de/teaching/ws13/mapping/
"機器人學一 (Robotics (1))" {NTU} 林沛群: https://www.coursera.org/learn/robotics1
"Control of Mobile Robots" {Georgia Tech} Magnus Egerstedt: https://www.coursera.org/learn/mobile-robot"
"Modern Robotics: Mechanics, Planning, and Control" {Northwestern University} Kevin Lynch: https://www.coursera.org/specializations/modernrobotics
"Robotics" {UPenn} https://zh-tw.coursera.org/specializations/robotics
"Linear algebra" {NTU} Hung-yi Lee: http://speech.ee.ntu.edu.tw/~tlkagk/courses_LA18.html
"Linear algebra" {MIT} Gilbert Strang: https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/
"Machine Learning" {NTU} Hung-yi Lee: http://speech.ee.ntu.edu.tw/~tlkagk/courses_ML19.html
"Probabilistic Systems Analysis and Applied Probability" {MIT} John Tsitsiklis https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-041-probabilistic-systems-analysis-and-applied-probability-fall-2010/"
"Deep Reinforcement Learning" {UCB} Sergey Levine: http://rail.eecs.berkeley.edu/deeprlcourse/
"Vision Algorithms for Mobile Robotics" {ETHZ} 	D. Scaramuzza: http://rpg.ifi.uzh.ch/teaching.html
"Self-Driving Cars" {TORONTO} https://www.coursera.org/specializations/self-driving-cars
```
Papers:
```js
"IEEE Xplore Digital Library": https://ieeexplore.ieee.org/Xplore/home.jsp
"arXiv.org e-Print archive": https://arxiv.org/
"Google Scholar": https://scholar.google.com/
```

## 1_ROS
ROS blogs&channel:  
```js
"半閒居士"： https://www.cnblogs.com/gaoxiang12/
"MR.POJENLAI": https://pojenlai.wordpress.com/
"The construct": https://www.youtube.com/channel/UCt6Lag-vv25fTX3e11mVY1Q
"泡泡機器人": https://space.bilibili.com/38737757/
"泡泡機器人論壇": http://paopaorobot.org/bbs/
```
Books:
```js
"ROS by Example", python, Patrick Goebel
"Mastering ROS for Robotics Programming", C++, Lentin Joseph
"Learning ROS for Robotics Programming", C++, Enrique Fernandez
"Programming Robots with ROS: A Practical Introduction to...", Morgan Quigley 
"机器人操作系统（ROS）浅析", Jason M. O'Kane著, 肖军浩译
"ROS 机器人操作系统ROS史话36篇", 张新宇, http://www.roseducation.org/docs/ROS_history.pdf
```
more: https://hackmd.io/s/B1fv26WBz# 

## 2_Robot_platform
ROS robots: https://robots.ros.org/  
holomic vs. non-holomic
```js
"Comparison": https://www.evernote.com/l/ATuaHlX8moZHApQrFpCNVYR4SlRPo8Tz53Y
"Caster wheel": https://en.wikipedia.org/wiki/Caster
"Mecanum wheel": https://en.wikipedia.org/wiki/Mecanum_wheel
"Omni wheel": https://en.wikipedia.org/wiki/Omni_wheel
```
race car project  
```js
"MIT": https://mit-racecar.github.io
"Penn": http://f1tenth.org/ [without slam, NAV]
"UCB": http://www.barc-project.com/projects/ [without laser] 
"Georgia Tech": https://github.com/AutoRally [for outdoor]
"Taiwan Hypharos": https://github.com/Hypha-ROS/hypharos_racecar
```
ROS mobile robot
```js
"turtlebot": https://github.com/turtlebot
"clearpath husky": https://github.com/husky
"clearpath jackel": https://github.com/jackal
```
ROS mobile manipulator
```js
"kuka youbot": https://github.com/youbot
"clearpath husky+UR5": http://www.clearpathrobotics.com/assets/guides/husky/HuskyManip.html
"clearpath husky+dualUR5": http://www.clearpathrobotics.com/assets/guides/husky/HuskyDualManip.html
```
processing unit: 
```
Raspberry Pi 3(RPi3), BeagleBone Black(BBB)
Odroid XU4, Odroid N2, Asus tinker board
NVIDIA Jetson TX1, NVIDIA Jetson TX2, NVIDIA Jetson NANO
```  
motor & controller:  ```Faulhaber, Maxon, Dexmart```  

## 3_Robot_sensor
RGB-camera:  
```js
"usb camera": http://wiki.ros.org/usb_cam
"gstream-based camera": http://wiki.ros.org/gscam
"opencv camera": http://wiki.ros.org/cv_camera
```
RGBD-camera:  
```js
"microsoft kinectv1 with openni": https://github.com/ros-drivers/openni_camera
"microsoft kinectv1 with freenect": https://github.com/ros-drivers/freenect_stack
"microsoft azure-kinect-dk": https://azure.microsoft.com/zh-tw/services/kinect-dk/
"asus xtion with openni2": https://github.com/ros-drivers/openni2_camera
"intel realsense d435": https://github.com/intel-ros/realsense
```
**Laser rangefinder** [laser scanners] [scanning rangefinder]  
– often represent 2D laser scanning
```js
"hokuyo_urg": http://wiki.ros.org/urg_node (old: http://wiki.ros.org/hokuyo_node
"hokuyo_utm": http://wiki.ros.org/urg_node (old: http://wiki.ros.org/hokuyo_node
"rplidar": http://wiki.ros.org/rplidar
"sick": http://wiki.ros.org/sick_scan
"ydlidar": https://github.com/YDLIDAR/ydlidar_ros
```
**LIDAR** [light detection and ranging] [light imaging, detection, and ranging] [3D laser scanning ]   
– often represent 3D laser scanning
```js
"velodyne": http://wiki.ros.org/velodyne
```
IMU:  
```js
"SparkFun 9DOF Razor IMUM0": http://wiki.ros.org/razor_imu_9dof
```
Odometry&3D scanning environment
```js
"Kaarta": https://www.kaarta.com/
"matterport": https://matterport.com/
```
Microphone array
```js
"microsoft azure-kinect-dk": https://azure.microsoft.com/zh-tw/services/kinect-dk/
"ReSpeaker Mic Array v2.0": http://wiki.seeedstudio.com/ReSpeaker_Mic_Array_v2.0/
```

## 4_odometry
ros pkg odometry
```
Wheel encoder and actuator | "ros_control": http://wiki.ros.org/ros_control
Laser odometry(old) | "laser_scan_matcher": http://wiki.ros.org/laser_scan_matcher
Laser odometry | "rf2o": https://github.com/MAPIRlab/rf2o_laser_odometry
```
sensor fusion ros pkg 
```
ekf | "robot_pose_ekf": http://wiki.ros.org/robot_pose_ekf
ekf&ukf | "robot_localization": http://docs.ros.org/melodic/api/robot_localization/html/index.html
```
#1#2 LOAM, V-LOAM, DEMO - lidar 
```
201905KITTI#1#2 - Laser Odometry and Mapping (Loam) is a realtime method for state estimation and mapping using a 3D lidar.
https://github.com/laboshinl/loam_velodyne
https://github.com/cuitaixiang/LOAM_NOTED
J Zhang, S Singh, "LOAM: Lidar Odometry and Mapping in Real-time", Robotics: Science and Systems Conference (RSS 2014)
J Zhang, S Singh, "Visual-lidar Odometry and Mapping: Low-drift, Robust, and Fast", IEEE International Conference on Robotics and Automation (ICRA)
J. Zhang, M. Kaess and S. Singh: Real-time Depth Enhanced Monocular Odometry. IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS) 2014.
```
#3#5 IMLS-SLAM, IMLS-SLAM++ - lidar
```
201905KITTI#3#5
Jean-Emmanuel Deschaud, "IMLS-SLAM: scan-to-model matching based on 3D data", arXiv:1802.08633 [cs.RO]
```
#4,17 SOFT, SOFT2 - Stereo 
```
201905KITTI#4,17 - Stereo Odometry based on careful Feature selection and Tracking. 
https://github.com/Mayankm96/Stereo-Odometry-SOFT
Cvišic, Igor, et al. "Soft-slam: Computationally efficient stereo visual slam for autonomous uavs." Journal of field robotics (2017).
Cvišić, Igor, and Ivan Petrović. "Stereo odometry based on careful feature selection and tracking." 2015 European Conference on Mobile Robots (ECMR). IEEE, 2015.
```
#10#19 RotRocc+, RotRocc, ROCC, MonoROCC - stereo?
```
201905KITTI#10#19
M. Buczko and V. Willert: Flow-Decoupled Normalized Reprojection Error for Visual Odometry. 19th IEEE Intelligent Transportation Systems Conference (ITSC) 2016.
M. Buczko, V. Willert, J. Schwehr and J. Adamy: Self-Validation for Automotive Visual Odometry. IEEE Intelligent Vehicles Symposium (IV) 2018.
M. Buczko: Automotive Visual Odometry. 2018.
M. Buczko and V. Willert: Monocular Outlier Detection for Visual Odometry. IEEE Intelligent Vehicles Symposium (IV) 2017.
M. Buczko and V. Willert: How to Distinguish Inliers from Outliers in Visual Odometry for High-speed Automotive Applications. IEEE Intelligent Vehicles Symposium (IV) 2016.
```
#11,13,23 LIMO_GP, LIMO2, LIMO - mono + lidar
```
201905KITTI#11,13,23 - Lidar-Monocular Visual Odometry
https://github.com/johannes-graeter/limo
Graeter, Johannes, Alexander Wilczynski, and Martin Lauer. "Limo: Lidar-monocular visual odometry." 2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, 2018.
```
#34 VINS - Stereo, mono, RGBD + inertial
```
201905KITTI#34 - An optimization-based multi-sensor state estimator
https://github.com/HKUST-Aerial-Robotics/VINS-Fusion
https://github.com/HKUST-Aerial-Robotics/VINS-Mono
Online Temporal Calibration for Monocular Visual-Inertial Systems, Tong Qin, Shaojie Shen, IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS, 2018), best student paper award pdf
VINS-Mono: A Robust and Versatile Monocular Visual-Inertial State Estimator, Tong Qin, Peiliang Li, Zhenfei Yang, Shaojie Shen, IEEE Transactions on Roboticspdf
```
#40 ORB-SLAM2 - Stereo, mono, RGBD
```
201905KITTI#40 - Real-Time SLAM for Monocular, Stereo and RGB-D Cameras, with Loop Detection and Relocalization Capabilities
https://github.com/raulmur/ORB_SLAM2
[Monocular] Raúl Mur-Artal, J. M. M. Montiel and Juan D. Tardós. ORB-SLAM: A Versatile and Accurate Monocular SLAM System. IEEE Transactions on Robotics, vol. 31, no. 5, pp. 1147-1163, 2015. (2015 IEEE Transactions on Robotics Best Paper Award). PDF.
[Stereo and RGB-D] Raúl Mur-Artal and Juan D. Tardós. ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras. IEEE Transactions on Robotics, vol. 33, no. 5, pp. 1255-1262, 2017. PDF.
[DBoW2 Place Recognizer] Dorian Gálvez-López and Juan D. Tardós. Bags of Binary Words for Fast Place Recognition in Image Sequences. IEEE Transactions on Robotics, vol. 28, no. 5, pp. 1188-1197, 2012. PDF
```
#48 VoBa - IMU, visual-aided
```
201905KITTI#48
J. Tardif, M. George, M. Laverne, A. Kelly and A. Stentz: A new approach to vision-aided inertial navigation. 2010 IEEE/RSJ International Conference on Intelligent Robots and Systems, October 18-22, 2010, Taipei, Taiwan 2010.
```
#54 RTAB-Map - RGB-D, Stereo and Lidar
```
A RGB-D, Stereo and Lidar Graph-Based SLAM approach based on an incremental appearance-based loop closure detector. 
M. Labbé and F. Michaud, “RTAB-Map as an Open-Source Lidar and Visual SLAM Library for Large-Scale and Long-Term Online Operation,” in Journal of Field Robotics, vol. 36, no. 2, pp. 416–446, 2019. (Wiley) Universit ́e de Sherbrooke
http://introlab.github.io/rtabmap/
```
DeepVO - learning_based: RGB
```
S. Wang, R. Clark, H. Wen and N. Trigoni, "DeepVO: Towards end-to-end visual odometry with deep Recurrent Convolutional Neural Networks," 2017 IEEE International Conference on Robotics and Automation (ICRA), Singapore, 2017, pp. 2043-2050.
https://github.com/ChiWeiHsiao/DeepVO-pytorch
https://github.com/ildoonet/deepvo
https://github.com/krrish94/DeepVO
https://github.com/linjian93/pytorch-deepvo
```
VINET - learning_based: RGB + IMU
```
Clark, Ronald, et al. "VINet: Visual-Inertial Odometry as a Sequence-to-Sequence Learning Problem." AAAI. 2017.
https://github.com/HTLife/VINet
```

## 5_SLAM
The classical SLAM theorem
```
T. Bailey and H. F. Durrant-Whyte, “Simultaneous localisation and map- ping (SLAM): Part II”, IEEE Robot. Auton. Syst., vol. 13, no. 3, pp. 108–117, 2006. 
H. F. Durrant-Whyte and T. Bailey, “Simultaneous localisation and map- ping (SLAM): Part I”, IEEE Robot. Autom. Mag., vol. 13, no. 2, pp. 99–110, Jun. 2006
```
Survey paper
```
Cesar Cadena ; Luca Carlone ; Henry Carrillo ; Yasir Latif ; Davide Scaramuzza ; José Neira ; Ian Reid ; John J. Leonard
, “Past, Present, and Future of Simultaneous Localization And Mapping: Towards the Robust-Perception Age”, IEEE Transactions on RoboticsYear: 2016, Volume: 32, Issue: 6Pages: 1309 - 1332
```
Cartographer - odom + rangeSensor + IMU
```
Wolfgang Hess ; Damon Kohler ; Holger Rapp ; Daniel Andor, “Real-time loop closure in 2D LIDAR SLAM ”, 2016 IEEE International Conference on Robotics and Automation (ICRA), Stockholm, 2016, pp. 1271-1278.
https://github.com/googlecartographer/cartographer
https://github.com/googlecartographer/cartographer_ros
```
#54 RTAB-Map - RGB-D, Stereo and Lidar
```
A RGB-D, Stereo and Lidar Graph-Based SLAM approach based on an incremental appearance-based loop closure detector. 
M. Labbé and F. Michaud, “RTAB-Map as an Open-Source Lidar and Visual SLAM Library for Large-Scale and Long-Term Online Operation,” in Journal of Field Robotics, vol. 36, no. 2, pp. 416–446, 2019. (Wiley) Universit ́e de Sherbrooke
http://introlab.github.io/rtabmap/
```
Gmapping - http://wiki.ros.org/gmapping
```
G. Grisetti, C. Stachniss and W. Burgard, "Improved Techniques for Grid Mapping With Rao-Blackwellized Particle Filters," IEEE Transactions on Robotics, vol. 23, no. 1, pp. 34-46, Feb. 2007.
```


## 6_Localization
amcl Adaptive (or KLD-sampling) Monte Carlo localization: http://wiki.ros.org/amcl  
mrpt_localization: http://wiki.ros.org/mrpt_localization  
google_cartographer: https://google-cartographer-ros.readthedocs.io/en/latest/demos.html#pure-localization


## 7_Map
OctoMap - 3D occupancy mapping: https://octomap.github.io/
```
Hornung, Armin & Wurm, Kai & Bennewitz, Maren & Stachniss, Cyrill & Burgard, Wolfram, "OctoMap: An efficient probabilistic 3D mapping framework based on octrees. Autonomous Robots.", Autonomous Robots Journal (2013). 34. 10.1007/s10514-012-9321-0. 
```


## 8_Navigation_moveBase
(move_base compatible, nav_core supported)  
dwa_local_planner, base_local_planner http://wiki.ros.org/dwa_local_planner
```
D. Fox, W. Burgard and S. Thrun, "The dynamic window approach to collision avoidance," in IEEE Robotics & Automation Magazine, vol. 4, no. 1, pp. 23-33, March 1997.
```
teb_local_planner http://wiki.ros.org/teb_local_planner
```
C. Rösmann, F. Hoffmann and T. Bertram: Integrated online trajectory planning and optimization in distinctive topologies, Robotics and Autonomous Systems, Vol. 88, 2017, pp. 142–153.
C. Rösmann, W. Feiten, T. Wösch, F. Hoffmann and T. Bertram: Trajectory modification considering dynamic constraints of autonomous robots. Proc. 7th German Conference on Robotics, Germany, Munich, May 2012, pp 74–79.
C. Rösmann, W. Feiten, T. Wösch, F. Hoffmann and T. Bertram: Efficient trajectory optimization using a sparse model. Proc. IEEE European Conference on Mobile Robots, Spain, Barcelona, Sept. 2013, pp. 138–143.
C. Rösmann, F. Hoffmann and T. Bertram: Planning of Multiple Robot Trajectories in Distinctive Topologies, Proc. IEEE European Conference on Mobile Robots, UK, Lincoln, Sept. 2015.
C. Rösmann, F. Hoffmann and T. Bertram: Kinodynamic Trajectory Optimization and Control for Car-Like Robots, IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Vancouver, BC, Canada, Sept. 2017.
Source code: https://github.com/rst-tu-dortmund/teb_local_planner
```
navigation_stack: http://wiki.ros.org/navigation  
```js
"local_planner": base_local_planner, dwa_local_planner, eband_local_planner, teb_local_planner, robotino_local_planner, asr_ftc_local_planner, simple_local_planner  
"global_planner": carrot_planner, navfn, global_planner, sbpl_lattice_planner, srl_global_planner, voronoi_planner
"RecoveryBehavior": rotate_recovery, move_slow_and_clear, stepback_and_steerturn_recovery
```

## 9_Navigation_advanced
condition keywords: ```in crowded spaces, in cluttered environments, socially aware```
```
MIT AerospaceControlsLab
Y. F. Chen, M. Liu, M. Everett and J. P. How "Decentralized non-communicating multiagent collision avoidance with deep reinforcement learning," 2017 IEEE International Conference on Robotics and Automation (ICRA), Singapore, 2017, pp. 285-292. 
https://www.youtube.com/watch?v=PS2UoyCTrSw
https://www.youtube.com/watch?v=BryJ9jeBkbU
```
```
MIT AerospaceControlsLab
Y. F. Chen, M. Everett, M. Liu and J. P. How, "Socially aware motion planning with deep reinforcement learning," 2017 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Vancouver, BC, 2017, pp. 1343-1350.
https://www.youtube.com/watch?v=CK1szio7PyA&t=2s
```
```
MIT AerospaceControlsLab
M. Everett, Y. F. Chen and J. P. How, "Motion Planning Among Dynamic, Decision-Making Agents with Deep Reinforcement Learning," 2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Madrid, Spain, 2018, pp. 3052-3059.
https://www.youtube.com/watch?v=XHoXkWLhwYQ
```
```
Google AI Research
A. Faust et al., "PRM-RL: Long-range Robotic Navigation Tasks by Combining Reinforcement Learning and Sampling-Based Planning," 2018 IEEE International Conference on Robotics and Automation (ICRA), Brisbane, QLD, 2018, pp. 5113-5120.
Francis, Anthony & Faust, Aleksandra & Chiang, Hao-Tien Lewis & Hsu, Jasmine & Chase Kew, J & Fiser, Marek & Edward Lee, Tsang-Wei. (2019). Long-Range Indoor Navigation with PRM-RL. 
H. L. Chiang, A. Faust, M. Fiser and A. Francis, "Learning Navigation Behaviors End-to-End With AutoRL," in IEEE Robotics and Automation Letters, vol. 4, no. 2, pp. 2007-2014, April 2019.
https://ai.googleblog.com/2019/02/long-range-robotic-navigation-via.html
```
```
ETHz Autonomous System Lab
M. Pfeiffer, U. Schwesinger, H. Sommer, E. Galceran and R. Siegwart, "Predicting actions to act predictably: Cooperative partial motion planning with maximum entropy models," 2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Daejeon, 2016, pp. 2096-2101.
https://www.youtube.com/watch?v=GPp5mnybm8g
```

## 10_Others_Non_tech_part
### (1) Famous robotics related company
Research center: ```Toyota_Research_Institute(TRI), Microsoft_Research, Google_AI```  
Manipulator: ```ABB, FANUC, KUKA, YASKAWA, TECHMAN_ROBOT, HIWIN, Universal_robots  ```  
Mobile Robot(AGV, base only): ```omron_robotics, clearpath_robotics&OTTO_Motors, amazon_robotics(Kiva_System), Yujin_Robotics, ROBOTIS, fetch_robotics, GreenTrans, KUKA, iRobot, pal_robotics, Robotnik_Automation```  
Service robot(with torso): ```willow_garage, softbank_robotics, fetch_robotics, pal_robotics, Robotnik_Automation```  
Humanoid: ```boston_dynamics, softbank_robotics, pal_robotics```  
Quadruped: ```boston_dynamics, unitree_robotics, MIT_Cheetah, ANYrobotics(ANYmal), Standford＿Doggo```  
Drone: ```Dji, Tello```  
ROS2.0: ```ADLINK ```  
Cleaning: ```iRobot```  
Gripper: ```ROBOTIQ```  
Self-Driving Cars : ```Alphabet Waymo, Uber, Apple Project Titan```  

### (2) Famous robotics conferences & journals
Top conference: ```IROS, ICRA```  
Top journal: ```IEEE_Transactions_on_Robotics_and_Automation, IEEE_Transactions_on_Robotics```  
Minor conference:```IECON, SII, ISIE, ICIT, ICPS```  
Minor journal: ```IEEE_Access```  
The IEEE Robotics and Automation Society: https://www.ieee-ras.org/conferences-workshops  
The Industrial Electronics Society: http://www.ieee-ies.org/conferences  
google scholar rank: https://scholar.google.com/citations?view_op=top_venues&hl=en&vq=eng_robotics  

### (3) Famous robotics competition
Global:
```js
"DARPA Robotics Challenge": https://en.wikipedia.org/wiki/DARPA_Robotics_Challenge
"RoboCup": https://en.wikipedia.org/wiki/RoboCup
"Amazon Robotics/Picking Challenge": http://amazonpickingchallenge.org/
"ICRA Robot Competitions: including lots of competitions would be different every years"
"IROS Robot Competitions: including lots of competitions would be different every years"
```
In Taiwan:
```js
"SKS 新光保全智慧型保全機器人競賽": https://www.facebook.com/sksrobot/
"PMC 智慧機器人競賽 Robot competition": http://www.pmccontest.com/
"HIWIN 上銀智慧機械手實作競賽": http://www.hiwin.org.tw/Awards/HIWIN_ROBOT/Original.aspx
"SiliconAwards 旺宏金矽獎"http://www.mxeduc.org.tw/SiliconAwards/
```

### (4) Famous ros organizations & activities
ros related work:
```js
"ROS-industrial": https://rosindustrial.org/
"ROS2.0": https://design.ros2.org/
"ROS-H": https://acutronicrobotics.com/technology/H-ROS/"
```
organizations:
```js
"Open Source Robotics Foundation (OSRF)": https://www.openrobotics.org/
"Open Source Robotics Corporation (OSRC)": https://www.openrobotics.org/
"ROS.Taiwan": https://www.facebook.com/groups/ros.taiwan/
"ROS.Taipei": https://www.facebook.com/groups/ros.taipei/
```
activities: 
```js
"ROScon": https://roscon.ros.org/
"ROSDevCon": http://www.theconstructsim.com/ros-developers-online-conference-2019-rdc-worldwide/
"ROS summer school(CN)": http://www.roseducation.org/
```
