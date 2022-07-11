### ****Steps to downlaod ROS****

1-	Downlaod Virtual box version 6.1.34

2-	Download Ubuntu version 20.04.4

3-	Open the Virtual box and press new to create virtual system choose Ubuntu-64bit and change the memory size to 5000 MG and the hard disk and the size of virtual to 50 GB

4-	Go to the settings and change some options such as change the processor to 4 CPU and upload the disk file we download it before
After those steps I had a proplem when I pressed start button an error message appears, the error code is 0x80004005 I solved the proplem by two steps :
-	I changed the BIOS setting and let Virtualization Technology >Enabled<
-	I pressed the arrow next to start button on Virtual box and then pressed Headless start and then Show button

5-	After the system opened Install Ubuntu 
 
6-	Restart the system

7-	Go to the terminal and write those instrucation:

### Setup the sourceslist

`sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'`

### Set up the keys

`sudo apt install curl # if you haven't already installed curl`
`curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -`

### Installation
`sudo apt update` 

### Desktop Install

`sudo apt install ros-noetic-desktop`

### Environment setup

``source /opt/ros/noetic/setup.bash``


8- To be sure that ROS is installed 
Write roscore on the terminal



