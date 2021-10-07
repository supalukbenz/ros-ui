# ROS GUI

ROS GUI is a web browser tool for communicating and controlling robots via [ROS](http://wiki.ros.org/Documentation). The interaction between the browser and ROS uses [roslibjs](https://github.com/RobotWebTools/roslibjs) with the WebSockets as an intermediary. 

## Requirements

Before using this project, make sure that the robot has the following packages:

1. [rosbridge_suite](http://wiki.ros.org/rosbridge_suite) is a specification for sending JSON based commands to ROS.
   - Rosbridge is available as a debian. To install:

     ```sudo apt-get install ros-<rosdistro>-rosbridge-server```

2. [web_video_server](http://wiki.ros.org/web_video_server) provides a video stream of a ROS image transport topic that can be accessed via HTTP.
   - Install web_video_server Screen on Ubuntu and Debian

     ```sudo apt-get install ros-<rosdistro>-web-video-server```

3. **screen** is a terminal multiplexer for launching and using multiple shell sessions from a single ssh session.
   - Install Linux Screen on Ubuntu and Debian

     ```sudo apt install screen```

## Project installation

Clone the repository and install dependencies:
    
```bash
$ https://github.com/supalukbenz/ros-gui.git
$ cd ros-gui 
$ npm install
```

Run the project
```bash
$ npm run serve
```

Open the ROS UI project at [http://localhost:8080/](http://localhost:8080/)


***In case of starting the backend server manually**

   - Go and follow the instructions at [https://github.com/supalukbenz/ros-gui-backend](https://github.com/supalukbenz/ros-gui-backend)

## Features
**1. Realtime graph**: Display values from selected ROS topics on a line graph in real-time.

**2. Streaming video**: Stream video of ROS image topic.

**3. Customize button**: Create and customize buttons to control or subscribe robot.

