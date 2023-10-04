<!-- TOC ignore:true -->
**Robot Dynamics Course Project**

**Table of Contents**
<!-- TOC -->

- [Setting up the Environment](#setting-up-the-environment)

<!-- /TOC -->
<!-- /TOC -->

# Setting up the Environment

We have ROS2 Humble as our base ROS Environment on which we are using Gazebo and RVIZ for simulations.

Add proprietary permissions to the script

```bash
sudo chmod u+x setup_script.sh
```

Execute the script

```bash
./setup_script.sh
```

Press the `Y` or `<password>` when prompted.

# Running Files

## Build the Project

In the home directory, build the project using

```bash
colcon build
```

Source the Environment

- For ZSH
    ```zsh
    source install/setup.zsh
    ```

- For BASH
    ```bash
    source install/setup.bash
    ```

## Launching the URDF Files

Run the xacro as:

```bash
ros2 launch pkg_manipulator manipulator.launch.py
```

Launch RVIZ as :

```bash
rviz2
```