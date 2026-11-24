# Autonomous Warehouse Robot — ROS 2 Jazzy

An open-source, simulation-based autonomous mobile robot (AMR) project built using ROS 2 Jazzy, C++ and Gazebo Harmonic.

This repository documents the step-by-step development of an autonomous warehouse robot, from workspace setup and robot modelling to SLAM, autonomous navigation and mission management.

The project is designed as both a practical robotics implementation and a learning resource for anyone interested in ROS 2 and autonomous mobile robots.

## Project Status

🚧 Under active development. Documentation and source code will be updated as the project progresses.

## Project Objectives

- Build a custom differential-drive mobile robot.
- Design a simulated warehouse environment.
- Integrate simulated LiDAR and wheel odometry.
- Generate maps using SLAM Toolbox.
- Implement localization using AMCL.
- Enable autonomous navigation using Nav2.
- Implement multi-station delivery missions using C++.
- Implement obstacle avoidance and navigation recovery.
- Test and evaluate robot performance.

## Technology Stack

| Technology | Purpose |
|---|---|
| Ubuntu 24.04 | Operating system |
| ROS 2 Jazzy | Robotics middleware |
| C++17 | Robot application development |
| Python | Launch files and supporting tools |
| Gazebo Harmonic | Robot simulation |
| RViz2 | Visualization |
| URDF / Xacro | Robot description |
| ros2_control | Robot control |
| SLAM Toolbox | Mapping |
| AMCL | Localization |
| Nav2 | Autonomous navigation |
| Git | Version control |

## Prerequisites

- Ubuntu 24.04 LTS
- ROS 2 Jazzy
- Gazebo Harmonic
- Basic ROS 2 knowledge
- Basic C++ programming knowledge

No physical robot or additional hardware is required.

## Tutorial — Build from Scratch

Each lesson explains the concept, its purpose, implementation, industry applications and common troubleshooting methods.

| Lesson | Topic | Status |
|---|---|---|
| 01 | [Workspace and package setup](docs/01-workspace-setup.md) | In progress |
| 02 | Warehouse environment | Planned |
| 03 | Robot description and sensors | Planned |
| 04 | ros2_control integration | Planned |
| 05 | SLAM mapping | Planned |
| 06 | AMCL localization | Planned |
| 07 | Nav2 autonomous navigation | Planned |
| 08 | Costmaps and path planning | Planned |
| 09 | Waypoint navigation | Planned |
| 10 | C++ mission manager | Planned |
| 11 | Fault handling and recovery | Planned |
| 12 | System testing and evaluation | Planned |

## Package Architecture

| Package | Responsibility |
|---|---|
| warehouse_description | Robot URDF, Xacro and sensor descriptions |
| warehouse_gazebo | Warehouse worlds and simulation |
| warehouse_bringup | Launch files and system configuration |
| warehouse_navigation | Mapping, localization and navigation |
| warehouse_missions | C++ mission management and delivery tasks |

## Installation and Execution

Complete installation and execution instructions will be added as the implementation progresses.

To build the workspace after setting up the required dependencies:

```bash
source /opt/ros/jazzy/setup.bash

cd ~/warehouse_ws

rosdep install --from-paths src --ignore-src -r -y

colcon build --symlink-install

source install/setup.bash
```

## Industry Applications

This project explores concepts used in:

- Autonomous mobile robots (AMRs)
- Warehouse automation
- Material transportation
- Industrial logistics
- Autonomous delivery systems

## Related Learning Resources

[ROS 2 Jazzy Robotics Roadmap](https://github.com/charles-shaju/ros2-jazzy-robotics-roadmap)

## License

License to be added.