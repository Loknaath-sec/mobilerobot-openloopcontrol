# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

### 1. Import Necessary Libraries:
  ~ Import the robot, time, and camera modules from the robomaster library to interact with the robot's components.

### 2. Initialize the Robot:
  ~ Create an instance of the robot.Robot() class to represent the robot.
  ~ Initialize the robot's connection using ep_robot.initialize(conn_type="ap").

### 3. Access Robot Components:
Create objects for the robot's chassis, LEDs, and camera:
  ~ ep_chassis = ep_robot.chassis
  ~ ep_led = ep_robot.led
  ~ ep_camera = ep_robot.camera

### 4. Perform Actions:
Start video stream:
  ~ Start streaming video from the robot's camera using ep_camera.start_video_stream(display=True, resolution=camera.STREAM_360P).
Move and change LEDs:
  ~ Execute a series of movements in a pre-defined pattern using ep_chassis.move().
  ~ Simultaneously change LED colors using ep_led.set_led() to create visual effects.
Stop video stream:
  ~ After a delay of 4 seconds, stop the video stream using ep_camera.stop_video_stream().

### Close the Connection:
  ~ Terminate the connection to the robot using ep_robot.close().


## Program
```python
from robomaster import robot
import time

if __name__ == '__main__':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis

    ## Write your code here



    
    ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)

Insert image here


<br/>
<br/>
<br/>
<br/>

## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)

<br/>
<br/>
<br/>
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
