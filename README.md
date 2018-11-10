# cartographer_ydlidar

## Usage
1. Install Cartographer to ~/catkin_ws  
<https://google-cartographer-ros.readthedocs.io/en/latest/compilation.html>

```
$ echo "source ~/catkin_ws/devel_isolated/setup.bash" >> ~/.bashrc
```

2. Install ydlidar to ~/user_ws  
<http://www.ydlidar.com/download>

```
$ mkdir -p ~/user_ws/src
$ cd ~/user_ws
$ catkin_make
$ source ~/user_ws/devel/setup.bash

$ cd ~/user_ws/src
$ git clone https://github.com/EAIBOT/ydlidar
$ cd ..
$ catkin_make --pkg ydlidar
```

```
$ source ~/user_ws/devel/setup.bash
$ roscd ydlidar/startup
$ sudo chmod 0777 *
$ sudo sh initenv.sh
```

3. Install cartographer_ydlidar (this repository)  

```
$ cd ~/user_ws/src
$ git clone https://github.com/Tokunn/cartographer_ydlidar
$ cd ..
$ catkin_make 
$ source ~/user_ws/devel/setup.bash
``


```
$ echo "source ~/user_ws/devel/setup.bash" >> ~/.bashrc
$ source ~/.bashrc
```

```
$ roslaunch cartographer_ydlidar ydlidar_2d.launch
```
