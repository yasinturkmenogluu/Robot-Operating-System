# ROS Kinetic Installation on Ubuntu 16.04

### 1. Set the computer to accept software from packages.ros.org <br/>
`$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'` <br/>

### 2. Set the keys <br/>
`$ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654` <br/>

### 3. Update packages <br/>
`$ sudo apt-get update` <br/>

### 4. Download Ros Kinetic full version
`$ echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc` <br/>
`$ source ~/.bashrc` <br/>
`$ source /opt/ros/kinetic/setup.bash` <br/>

### 5. Source ROS environment variables
`$ rosinstall` is a command line tool that allows you to easily download many source trees for ROS packages with a single command.
To install this tool and other dependencies for building ROS packages, run: <br/>
`$ sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential` <br/>

### 6. Install rosdep
You need to start rosdep before using many ROS tools. Rosdep allows you to easily install system dependencies for the source you want to compile and is required to run some core components in ROS.
`$ sudo apt install python-rosdep` <br/>

### 7. Run the commands below to start rosdep
`$ sudo rosdep init` <br/>
`$ rosdep update` <br/>
