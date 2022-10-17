# tii_ws
Workspace for camera network demo at TII

Build and source
```
git clone https://github.com/zp-yang/tii_ws.git
cd tii_ws
git submodule upate --init
colcon build
. install/setup.bash
```

In `src/qualisys_ros/launch/mocap.launch.py` change the arguments
`--server` (ip address) and `--rate` (hz) to match your system

To run the mocap node

`ros2 launch qualisys_ros mocap.launch.py`


To run real cameras, in a different terminal, source the workspace and run

`ros2 launch visnet gscam.launch.py`
