# LineFollowerRobot #

This repository is dedicated to the line follower project for the Introduction to Robotics course, taken in the 3rd year (2022-2023) at the Faculty of Mathematics and Computer Science, University of Bucharest. The project was made in teams of 2 people; I took part in the Runtime Terror team, along with @vladfxstoader.
## Components 

* Arduino Uno
* Zip-ties
* LiPo battery
* Two wheels
* Wires for the line sensor
* QTR-8A reflectance sensor
* Ball caster
* Extra wires 
* Chassis
* Breadboard
* L293D motor driver
* Two DC motors 


## Task

Implement a line follower robot able to follow a route which contains both straight lines and curves. The calibration should be done with automatic motor movement. In order to get the highest grade, the robot must complete the final track in less than 20 seconds. Our robot finished the track in 17.046 seconds. 

## Implementation

The automatic calibration of the sensors was implemented by moving the robot left and right along the axis according to the values read by the sensor. If the data from the sensors indicated that the robot was in the right side, it would move left, and if the robot was in the left side, it would move right.

The speed of the motors is controlled by the PID control, and the values which worked best for the constants KP, KI and KD were found empirically and their values were 8, 0.0001 and, respectively, 2. Also, the motors can also move in reverse if necessary, thus being able to take more sharp turns.

In order to get bonus points, we added two RGB LEDs that can be used as headlights.

## Setup Pictures
![alt text](https://github.com/ralucsandu/LineFollowerRobot/blob/main/setup-picture1.jpg?raw=true)
![alt text](https://github.com/ralucsandu/LineFollowerRobot/blob/main/setup-picture2.jpg?raw=true)

## Video Demo
https://www.youtube.com/watch?v=BLIfTCom64k
