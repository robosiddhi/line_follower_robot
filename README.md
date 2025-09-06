LINE FOLLOWING ROBOT
--------------------

A simple autonomous robot that follows a line using infrared sensors. 
It controls its motors to adjust movement and stay on track.

FEATURES
--------
- Detects and follows a black line on a white surface (or vice versa)
- Two DC motors for movement (differential drive)
- Uses IR sensors for detection
- Easy to build and test

COMPONENTS
----------
- 2 x DC motors with wheels
- Motor driver module (L298N or L293D)
- 2 x IR sensors (or more for higher accuracy)
- Microcontroller (Arduino, ESP, etc.)
- Robot chassis with caster wheel
- Battery pack

WORKING PRINCIPLE
-----------------
- IR sensors detect whether the surface is black (line) or white (background)
- Microcontroller processes sensor input
- Motor driver powers and controls the motors
- Robot adjusts its direction to follow the line

MOTOR DIRECTIONS
----------------
Sensor Left = White, Sensor Right = White  -->  Both motors forward
Sensor Left = Black, Sensor Right = White  -->  Turn left (right motor forward, left motor stop)
Sensor Left = White, Sensor Right = Black  -->  Turn right (left motor forward, right motor stop)
Sensor Left = Black, Sensor Right = Black  -->  Stop or treat as junction

APPLICATIONS
------------
- Educational robotics
- Robotics competitions
- Automated guided vehicles (AGVs)
- Line-based delivery robots
