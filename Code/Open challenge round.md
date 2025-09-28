Control software
====

* `Code of the open challenge round`

Purpose of the Program:
---

The main objective of this program is to enable the robot to behave autonomously and intelligently in an unfamiliar or dynamic environment. By using distance sensing and simple logic, the robot can:

-Detect and avoid obstacles.

-Choose optimal directions to continue moving.

-Stop safely when it reaches the end of its path.

This kind of program is often used in educational robotics projects to demonstrate basic concepts in autonomous navigation, sensor integration, and decision-making logic.

---
<img width="472" height="557" alt="image" src="https://github.com/user-attachments/assets/b06a27ef-0819-404b-901f-0e8c1fd3d1e1" />

---
Main Behaviors of the Robot:

1. Explores its surroundings while avoiding obstacles:

-As the robot moves forward, it continuously monitors its environment using an ultrasonic distance sensor.

-This sensor allows it to detect objects or walls within a specific range, helping it avoid collisions.

-The robot performs this detection in real-time, ensuring a responsive and adaptive behavior in changing environments.
---

2. Turns when it detects a nearby object (closer than 15 cm):

-If the robot identifies an obstacle in front of it at a distance of less than 15 centimeters, it recognizes this as a potential collision risk.

-To avoid the obstacle, the robot immediately decides to turn either left or right, depending on the available space.
---
3. Makes decisions based on which direction has more space (left or right):

-The robot checks the distances on both its left and right sides using additional sensor readings.

-If the left side is also blocked, it chooses to turn right.

-If the right side is blocked instead, it turns left.

-If both sides are obstructed, the robot defaults to turning right as a last resort.

-This decision-making process helps the robot navigate complex paths and confined spaces effectively.

---
5. Moves forward when no obstacles are detected nearby:

-If the robot detects no nearby obstacles (all distances greater than 15 cm), it continues moving forward in a straight line, advancing a fixed distance at a time (e.g., 10 cm).

-This ensures that the robot makes steady progress toward its destination or goal while remaining cautious of its surroundings.
---
5. Stops completely when it detects something very close (less than 5 cm):

-When the ultrasonic sensor detects an object closer than 5 centimeters, the robot interprets this as the end of the path, a wall, or the final goal.

-It then stops all movement, effectively ending its task and preventing any collisions.

-This behavior serves as a safety measure and a logical end condition for the program.

---





