**MOBILE ROBOTICS**

This repository contains Jupyter Notebooks (.ipynb files) detailing algorithm development for mapping, navigation, localization, and SLAM as part of the EECE5550 Mobile Robotics course.
*****************************************************************************************************************************************************************************************************
**Local Planning**

This notebook focuses on local trajectory generation and obstacle avoidance for a mobile robot. It implements interpolation techniques such as cubic splines and polynomial fitting to generate smooth and feasible trajectories. The approach ensures that the robot follows a collision-free path while maintaining dynamic feasibility. The notebook also includes reactive planning strategies such as the dynamic window approach (DWA) and potential field methods, which allow the robot to adapt its trajectory in real-time based on detected obstacles. Collision avoidance is a key aspect, ensuring that generated paths do not lead to unsafe conditions. The implementation uses numpy for numerical calculations and matplotlib for visualizing planned trajectories and obstacle regions. The robot's motion is constrained by velocity and acceleration limits, ensuring the generated paths are feasible given the robot's kinematic constraints. The notebook evaluates different local planning strategies, comparing their performance in terms of computational efficiency and trajectory smoothness. This implementation is crucial for enabling robots to navigate safely and efficiently in dynamic environments.
***************************************************************************************************************************************************************************************************
**Mapping and Localization**

This notebook contains implementations of particle filters and Monte Carlo localization methods for mobile robot pose estimation as well as occupancy grid mapping techniques. It demonstrates practical approaches to solving the robot localization problem in a known environment and the mapping problem in an unknown environment. The implementation utilizes particle-based Bayesian filtering for state estimation, LIDAR sensing models, and occupancy grid representations for mapping. The solutions are presented with detailed explanations, mathematical derivations, code implementations, and visualizations to illustrate the concepts and results.
*****************************************************************************************************************************************************************************************************
**Mobile Robot Kinematics and Control**

This notebook covers the mathematical modeling and control of mobile robots, focusing on kinematic equations that define their motion. It implements models such as the unicycle and differential drive kinematics, which describe how the robot's wheels influence its movement. The control strategies ensure that the robot follows a desired trajectory or reaches a target position accurately. The notebook includes implementations of PID control, Pure Pursuit, and Model Predictive Path Integral (MPPI) control to regulate the robot's motion. The implementation uses numpy for mathematical operations, matplotlib for visualizing trajectories and control responses, and symbolic computation to derive motion equations analytically. Simulations demonstrate how different control strategies affect the robot's ability to track a path accurately. The notebook also considers real-world constraints such as wheel slip and actuation limits, ensuring practical applicability. By integrating kinematics and control, this implementation provides a solid foundation for autonomous navigation, making it applicable to robotic vehicles, mobile platforms, and other autonomous systems.
*****************************************************************************************************************************************************************************************************
**Sensing and Coordinate Frames**

This notebook focuses on coordinate transformations and sensor integration for mobile robots. It implements homogeneous transformation matrices to convert between different coordinate frames, such as the world frame, robot frame, and sensor frames. These transformations are essential for accurate localization and mapping, ensuring that sensor data aligns with the robot's reference frame. The notebook processes LiDAR and vision sensor data to extract useful features such as object positions and obstacles. Sensor fusion techniques are applied to combine multiple sensor inputs, improving the reliability of perception. The implementation uses numpy for numerical computations and matplotlib for visualizing transformations and sensor readings. The notebook includes real-world examples and simulations that demonstrate how data from different sensors is transformed and interpreted. By accurately mapping sensor data to the robot's frame, this implementation enhances the robot's ability to perceive and navigate its environment effectively.
*****************************************************************************************************************************************************************************************************
**Simultaneous Localization and Mapping**

This assignment tackled the fundamental problem of Simultaneous Localization and Mapping (SLAM). The initial phase focused on point cloud registration, where the Iterative Closest Point (ICP) algorithm was implemented to align two sets of points by iteratively establishing correspondences and refining the transformation between them. This process is crucial for tasks like lidar odometry. The subsequent part introduced the concept of using factor graphs for state estimation in robotics. An odometry-based factor graph was constructed to estimate the robot's trajectory by incorporating a motion model and noisy sensor measurements. This approach leverages optimization techniques to find the most probable sequence of robot poses given the available information, forming the basis for a more comprehensive SLAM system.



