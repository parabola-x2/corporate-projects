# Terrain Mapping with LiDAR

The construction industry sought to enhance both safety and operational efficiency through workflow automation. The project involved equipping heavy machinery, such as dozers, with sensors capable of detecting soil stockpiles and distributing material evenly across surfaces. This was achieved by integrating LIDAR, GNSS, IMU, and gyroscope sensors onto the machinery. The LIDAR created a point cloud, and the IMUs corrected the PCL data depending on the position and orientation of the vehicle. Initially, operators manually controlled the equipment to gather training data, which was subsequently used to train a reinforcement learning algorithm. This algorithm could then be deployed on the machine to autonomously replicate human driving patterns, enabling the equipment to operate without human intervention.

Pose estimation was developed using MATLAB, while ROS was employed to process LIDAR data and apply pose correction. The final results were visualized using the Python library Open3D.

Extreme Programming (XP) was employed as the agile methodology to facilitate continuous customer engagement throughout evolving requirements and to accelerate development through pair programming. Upon reaching an acceptable level of software maturity, responsibility for further refinement was transitioned to my counterpart, who managed a separate component of the dozer development using the SCRUM framework with three-week sprint cycles.

<figure><img src=".gitbook/assets/bosch/traffic_light_2.png" alt=""><figcaption></figcaption></figure>



<figure><img src=".gitbook/assets/bosch/Autonomous Dozer.png" alt=""><figcaption></figcaption></figure>

I was responsible for end to end team coordination, and requirement gathering.

ROS, Matlab, Python, PCL, Unreal Engine, CARLA, IMU, Gyroscope, LiDAR, GNSS
