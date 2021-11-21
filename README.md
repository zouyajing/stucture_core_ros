
# structure_core_ros

Folked from https://github.com/chadrockey/structure_core_ros, and additional IMU topic is published.
The motivation is to use it as the device for RGB-D and inertial sensor fusion. Seems the quality is not good enough. 
Poor color and IMU. No time sync. 


To run and build:

1) From your Structure Core SDK download, copy the .so library from:

Libraries/Structure/Linux/x86_64 to lib/libStructure.so

2) Copy the ST folder from

Libaries/Shared/Headers to include/ST

into this repo.

Then run:

2) source /opt/ros/DISTRO/setup.bash
(source /opt/ros/kinetic/setup.bash or source /opt/ros/melodic/setup.bash)

3) catkin_make -DCMAKE_BUILD_TYPE=Release

Release is important or the code will not optimize correctly and may crash or run very poorly.