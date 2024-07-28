# Skid Steer ROS Bag Dataset

Dataset available under link:
https://drive.google.com/drive/folders/1grYkvnIKexDfoUioZt59QatlvPwNzBl7?usp=sharing
(github repository used for convenience)

## Dataset Description

This dataset contains ROS bag files collected during various trials of a skid steer robot on different surfaces. The directory structure is organized by surface types, wheel configurations, and test trajectories. Each subdirectory represents a specific surface type, each containing directories for different wheel configurations, which in turn contain subdirectories for two test trajectories (T1 and T2).

## Directory Structure

The dataset is organized as follows:

```plaintext
skid_steer
├── Artificial_grass_turf
│   ├── 4_1_1
│   │   ├── T1
│   │   └── T2
│   └── 6_1_1
│       ├── T1
│       └── T2
├── Carpet_15mm
│   ├── 4_1_1
│   │   ├── T1
│   │   └── T2
│   └── 6_1_1
│       ├── T1
│       └── T2
├── Carpet_6mm
│   ├── 4_1_1
│   │   ├── T1
│   │   └── T2
│   └── 6_1_1
│       ├── T1
│       └── T2
├── Ceramic_tiles
│   ├── 4_1_1
│   │   ├── T1
│   │   └── T2
│   └── 6_1_1
│       ├── T1
│       └── T2
├── EVA_rubber_foam
│   ├── 4_1_1
│   │   ├── T1
│   │   └── T2
│   └── 6_1_1
│       ├── T1
│       └── T2
├── Foam_underlayment_2mm
│   ├── 4_1_1
│   │   ├── T1
│   │   └── T2
│   └── 6_1_1
│       ├── T1
│       └── T2
├── Laminated_floor_panels
│   ├── 2_1
│   │   ├── T1
│   │   └── T2
│   ├── 2_2
│   │   ├── T1
│   │   └── T2
│   ├── 2_3
│   │   ├── T1
│   │   └── T2
│   ├── 4_1_1
│   │   ├── T1
│   │   └── T2
│   ├── 4_1_2
│   │   ├── T1
│   │   └── T2
│   ├── 4_1_3
│   │   ├── T1
│   │   └── T2
│   ├── 4_2_1
│   │   ├── T1
│   │   └── T2
│   ├── 4_2_2
│   │   ├── T1
│   │   └── T2
│   ├── 4_2_3
│   │   ├── T1
│   │   └── T2
│   ├── 4_3_1
│   │   ├── T1
│   │   └── T2
│   ├── 4_3_2
│   │   ├── T1
│   │   └── T2
│   ├── 4_3_3
│   │   ├── T1
│   │   └── T2
│   ├── 6_1_1
│   │   ├── T1
│   │   └── T2
│   ├── 6_1_2
│   │   ├── T1
│   │   └── T2
│   ├── 6_1_3
│   │   ├── T1
│   │   └── T2
│   ├── 6_2_1
│   │   ├── T1
│   │   └── T2
│   ├── 6_2_2
│   │   ├── T1
│   │   └── T2
│   ├── 6_2_3
│   │   ├── T1
│   │   └── T2
│   ├── 6_3_1
│   │   ├── T1
│   │   └── T2
│   ├── 6_3_2
│   │   ├── T1
│   │   └── T2
│   ├── 6_3_3
│   │   ├── T1
│   │   └── T2
│   ├── Tr1
│   │   ├── T1
│   │   └── T2
│   ├── Tr2
│   │   ├── T1
│   │   └── T2
│   └── Tr3
│       ├── T1
│       └── T2
├── Linoleum
│   ├── 4_1_1
│   │   ├── T1
│   │   └── T2
│   └── 6_1_1
│       ├── T1
│       └── T2
├── MDF_board
│   ├── 4_1_1
│   │   ├── T1
│   │   └── T2
│   └── 6_1_1
│       ├── T1
│       └── T2
└── PVC_foam
    ├── 4_1_1
    │   ├── T1
    │   └── T2
    └── 6_1_1
        ├── T1
        └── T2
```

## Surface Types

The top-level directories represent different surface types on which the skid steer robot was tested. These surfaces include:

- Artificial_grass_turf
- Carpet_15mm
- Carpet_6mm
- Ceramic_tiles
- EVA_rubber_foam
- Foam_underlayment_2mm
- Laminated_floor_panels
- Linoleum
- MDF_board
- PVC_foam

## Wheel Configurations

Within each surface type directory, the next level represents different wheel configurations used during the trials. Examples include:

- 4_1_1
- 6_1_1
- 2_1
- 2_2
- 2_3
- 4_1_2
- 4_1_3
- 4_2_1
- 4_2_2
- 4_2_3
- 4_3_1
- 4_3_2
- 4_3_3
- 6_1_2
- 6_1_3
- 6_2_1
- 6_2_2
- 6_2_3
- 6_3_1
- 6_3_2
- 6_3_3
- Tr1
- Tr2
- Tr3

## Test Trajectories

Each wheel configuration directory contains two subdirectories, T1 and T2, representing two different test trajectories for that particular configuration.

## Data Description

Each directory (T1, T2) within a wheel configuration contains ROS bag files of the trials. Each trial is named `trial_n.bag` where `n` is the trial number.

## ROS Bag File Details

Each ROS bag file contains sensor data recorded during a trial. Below is a typical description of a ROS bag file:

- **Path**: `trial_n.bag` (where `n` is the trial number)
- **Version**: 2.0
- **Duration**: 48.7 seconds
- **Start**: Jan 14 2023 12:38:55.91
- **End**: Jan 14 2023 12:39:44.58
- **Size**: 14.8 MB
- **Messages**: 62488
- **Compression**: None

### Topics and Message Types

The ROS bag files include various topics with different message types:

- `/Servo_data`: `kin_odom_msg/Measurements`
- `/cmd_vel`: `geometry_msgs/Twist`
- `/filter/quaternion`: `geometry_msgs/QuaternionStamped`
- `/imu/acceleration`: `geometry_msgs/Vector3Stamped`
- `/imu/angular_velocity`: `geometry_msgs/Vector3Stamped`
- `/imu/data`: `sensor_msgs/Imu`
- `/imu/mag`: `geometry_msgs/Vector3Stamped`
- `/imu/time_ref`: `sensor_msgs/TimeReference`
- `/odom`: `nav_msgs/Odometry`
- `/rosout`: `rosgraph_msgs/Log`
- `/rosout_agg`: `rosgraph_msgs/Log`
- `/tf`: `tf2_msgs/TFMessage`
- `/turtlebot_burger/odom`: `nav_msgs/Odometry`
- `/velocity`: `kin_odom_msg/VelocityWheel`
- `/vicon/turtlebot_burger`: `vicon/Subject`
- `/vicon/unlabeled_markers`: `vicon/Markers`

## Compression

The ROS bag files in this dataset are compressed using the bz2 method for long term storage. To decompress these files, use the following command:

```sh
rosbag decompress path/to/trial_n.bag
```

## Usage Instructions
To use this dataset, follow these steps:

Download the Dataset: Download the required ROS bag files from the directory corresponding to the surface type, wheel configuration, and test trajectory you are interested in.
Run Analysis: Use ROS tools (e.g., rosbag, rqt_bag) to analyze the bag files.
Visualize Data: Visualize the data using RViz or other suitable visualization tools.

## Contact Information
For any questions or further information, please contact:

lukasz.chlebowicz@dokt.p.lodz.pl
   

