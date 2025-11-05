# NAUTILUS [an ARIS project](https://aris-space.ch/our-projects/nautilus/).

## System Architecture
Our UUV uses a multi-component software system:
- **Mission Laptop**: Vue.js frontend + FastAPI backend for mission planning
    - [command-bridge-backend](https://github.com/Nautilus-UUV/command-bridge-backend), @jannick-schroeer @alisergoener
    - [command-bridge-frontend](https://github.com/Nautilus-UUV/command-bridge-frontend),
    @jannick-schroeer @alisergoener
- **RaspberryPi**: ROS2-based nodes for navigation and control
    - [uuv-ros](https://github.com/Nautilus-UUV/uuv-ros), @seemos
- **Main PCB**: FreeRTOS + microROS for CAN bus communication
- **Sensor PCB**: Low-level sensor data collection

## Simulations
- [dave](https://github.com/Nautilus-UUV/dave), @massarin: a fork of [IOES-Lab/dave](https://github.com/IOES-Lab/dave) (ros2 branch of [Field-Robotics-Lab/dave](https://github.com/Field-Robotics-Lab/dave)) that hosts our custom Polaris model

## Legacy
- [polaris-ros2-divetest](https://github.com/Nautilus-UUV/polaris-ros2-divetest), @ReasonableFailure: Integrated code for the 2025 divetest at Zürisee
- [dave-ros1](https://github.com/Nautilus-UUV/dave-ros1), @wueestry: a fork of ros1 dave, contains legacy meshes and custom mavros script
