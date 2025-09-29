Control Software
====

This program is designed to control a robot by combining different modules of instructions that allow it to move autonomously. The logic is divided into three main parts: the parking exit routine, the use of ultrasonic sensors to assist with turns, and decision-making with a color sensor.

----

* `Code of the obstacle challenge round`

<img width="550" height="627" alt="image" src="https://github.com/user-attachments/assets/8025022d-d154-4b7c-a238-200cf39de5a7" />

----

The first section of the program is dedicated to **exiting the parking spot**. In this routine, the motors are configured with specific speeds and positions, and the robot performs short forward and backward movements with pauses in between. This sequence allows the robot to align itself correctly and leave the initial area before starting its autonomous navigation.

----

<img width="254" height="633" alt="image" src="https://github.com/user-attachments/assets/8898f398-912e-4f08-b836-e1546c70bad2" />

----

Once the robot has exited the parking area, the second part of the program begins, which focuses on the use of **ultrasonic sensors**. These sensors are mainly activated during turns on the track. By measuring the distance to the walls, the robot can decide the best direction to follow. Each time it approaches a turning point, the sensors compare the available space on both sides, and the robot turns toward the side with greater clearance. This behavior is repeated consistently, ensuring that the robot adapts to the layout of the track and avoids collisions with the walls.

----

<img width="370" height="487" alt="image" src="https://github.com/user-attachments/assets/876ffbc5-e814-47c3-a7ce-553b9f018740" />

----

The third section of the program involves the **color sensor**, which is used to give the robot specific directional commands. When the sensor detects the color **red**, the robot executes a turn to the right. On the other hand, when the sensor detects the color **green**, the robot turns to the left. This is achieved by adjusting the motor speeds, moving to precise positions, and including short delays that guarantee smooth and controlled turns.

----

<img width="507" height="623" alt="image" src="https://github.com/user-attachments/assets/aece9033-e7bf-4d63-94a0-415dc70b953d" />

----

In conclusion, this program allows the robot to act autonomously by combining three levels of behavior. First, it leaves the parking spot through a programmed sequence of movements. Then, it uses ultrasonic sensors to determine the best path when turning on the track, always choosing the side with more space. Finally, it interprets color signals to perform additional directional decisions. Together, these elements demonstrate the integration of sensors and programming logic to achieve reliable and autonomous robotic navigation.
