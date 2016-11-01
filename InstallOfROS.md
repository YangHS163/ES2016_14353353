##LAB5

Mission: Installation of ROS jade
Reference: http://wiki.ros.org/jade/Installation/Ubuntu

##Command line

First: Setup your sources.list
*sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'*

Second: Installation (Buntu 14.04 )
*sudo apt-get update*
There are many different libraries and tools in ROS. And we should download the recommended one:
*sudo apt-get install ros-jade-desktop-full*
After installation, it will decompression automatically

Third: Environment setup
It's convenient if the ROS environment variables are automatically added to your bash session every time a new shell is launched:
*echo "source /opt/ros/jade/setup.bash" >> ~/.bashrc* 
*source ~/.bashrc*
If we have more than one ROS distribution installed, ~/.bashrc must only source the setup.bash for the version we are currently using. But this is our first time using ROS, so it is unnecessary.

At last: Getting rosinstall
*sudo apt-get install python-rosinstall*
THis is a frequently used command-line tool in ROS. And it is distributed separately and enables us to easily download many source trees for ROS packages with one command( So,I think it is unnecessary, too ).
