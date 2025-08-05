Download

Download the package by clicking the green Code button and press Download ZIP on Github. Extract the second_ros2 folder from the zip file into your home.
Build
Open terminal and enter the second_ros2 folder. Colcon build the urdf_robot package.

```bash
colcon build --packages-select urdf_robot
```

then source install

```bash
source install/setup/bash
```

then launch the ros2 state publisher

```bash
ros2 launch urdf_robot launch.py
```

finally make a new terminal while keeping the old one and now run the rviz

```bash
rviz2 -d install/urdf_robot/share/urdf_robot/urdf/my_robot.rviz
```
Now your done