# 1- Dependencies
{ sudo apt-get install ros-noetic-effort-controllers }

# 2- Simulator installation
{ cd }

{ mkdir -p baxterws/src }

{ cd baxterws/src/ }

{ wstool init }

{ wstool merge https://gist.githubusercontent.com/jarvisschultz/f65d36e3f99d94a6c3d9900fa01ee72e/raw/baxter_packages.rosinstall }

{ wstool update }

{ source /opt/ros/noetic/setup.bash }

{ cd .. }

{ catkin_make }

{ echo 'source ~/baxterws/devel/setup.bash'>>~/.bashrc }

{ source ~/.bashrc }


