# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1:

Initiate the MobileRobot

Step2:

Connect your PC with the MobileRobot.

Step3:

 Open Python program.

Step4:

Program the movements of the robot using python code.

Step5:

Execute the python program.

## Program :
Python control code to move the mobilerobot along the predefined path.

Developed by: MAMTHA I

Register No.: 212222230076

```
from robomaster import robot
import time
from robomaster import camera


if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

   
    
    ep_chassis.move(x=2.8, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=100,b=0,effect="on")


    ep_chassis.move(x=0 , y=0, z=50, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=255,b=204,effect="on")


    ep_chassis.move(x=0.4, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")


    ep_chassis.move(x=0, y=0, z=45, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=204,b=0,effect="on")


    ep_chassis.move(x=0.8, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=204,b=255,effect="on")


    ep_chassis.move(x=0, y=0, z=85, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=128,g=0,b=0,effect="on")



    ep_chassis.move(x=1.2, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

   
    ep_chassis.move(x=0, y=0, z=-45, xy_speed=1).wait_for_completed()

    ep_chassis.move(x=1.7, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=102,g=0,b=202,effect="on")


    ep_chassis.move(x=0, y=0, z=43, xy_speed=1).wait_for_completed()


    ep_chassis.move(x=1.4, y=0, z=0, xy_speed=1).wait_for_completed()

    ep_chassis.move(x=0, y=0, z=95, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")


    ep_chassis.move(x=2.2, y=0, z=0, xy_speed=1).wait_for_completed()

    ep_chassis.move(x=0, y=0, z=80, xy_speed=1).wait_for_completed()

    ep_led.set_led(comp = "all",r=255,g=102,b=0,effect="on")

    ep_chassis.move(x=0.6, y=0, z=0, xy_speed=1).wait_for_completed()

    time.sleep(4)
    
    
    p_camera.stop_video_stream()
    print("Stopped video streaming.....")
    ep_robot.close()
 ```
## MobileRobot Movement Image:

![robo](./img/robomaster.png)

## Starting point:
![243182096-33e31e8a-fbbe-42ca-9608-9a0277427cbf](https://github.com/Mamthaiyappaprabu/mobilerobot-openloopcontrol/assets/119393563/12b53294-6293-42a6-9544-5c4e7d7c4cc2)

## Turning point:
![243182121-58dca3ff-d6c2-4599-909f-e16c0cd91e7b](https://github.com/Mamthaiyappaprabu/mobilerobot-openloopcontrol/assets/119393563/97b29097-c9fd-44c4-a1eb-afc0dc392347)

## End point:
![243182135-bb341f7f-c54d-44fc-8c37-31f99cbec446](https://github.com/Mamthaiyappaprabu/mobilerobot-openloopcontrol/assets/119393563/05213b9c-0e4b-475d-a6b0-6c93d592c600)


## MobileRobot Movement Video:
https://youtu.be/xG8uLQ4aqBk


## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
