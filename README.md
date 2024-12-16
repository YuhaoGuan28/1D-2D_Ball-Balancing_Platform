Project Proposal – Ball balancing with PID control
Overview
The project aims to balance a ball on a square surface using the principles of PID control. The system will consist of a pressure-sensing plate/screen or a camera that detects the ball’s xy-coordinates on the surface and two servo motors that tilt the surface to prevent the ball from falling off the surface. The STM-32 microcontroller will serve as the controller.
The project consists of two parts. In the first part, the ball will be on a 1-dimensional (1D) guide rail as opposed to a 2-dimensional (2D) surface. The ball’s position will be detected using only an ultrasonic sensor. The rail, controlled only by one servo motor, will tilt clockwise or counterclockwise to prevent the ball from falling off the ends. If the first part is successful, we will implement the aforementioned second part.
We will implement the control code and assemble the mechanical structure. We will demonstrate how the system tilts the surface real-time to prevent the ball from falling during the lab session.

Background
The following resources are relevant projects that inspired our design decisions–using a servo motor and using a camera or pressure sensor–about potential structures and methods to complete the project:
-	1D ball balancing by Electronoobs (Infrared Sensor, servo motor, and PID): https://electronoobs.io/tutorial/11#
-	2D ball balancing by Moosenee (Touch resistive screen, servo motors, and PID): https://www.instructables.com/PID-Controlled-Ball-Balancing-Stewart-Platform/
-	2D ball balancing by Giusenso (Computer Vision Module, servo motors, and PID): https://github.com/giusenso/Ball-Balancing-PID-System

Designer experiences
This project mainly achieves 3 functions: checking ball’s position (BP), 1D/2D platform controlling (PC), and PID controlling algorithm (PID). Currently, our idea for BP is to use either Camera positioning (SCCB) or Force sensing positioning (USB). For PC, our idea is to use servo motors (controlled by PWM). Both steps require serial communication between the peripheral and microcontroller, which our experience in ECE342 and ECE295 will be useful. Meanwhile, we took ECE311 and ECE470 where we learnt the method of PID control.

Milestones
M1 - Mar22 - Researching, Material preparation, First part (1D) hardware setup & testing done
M2 - Mar29 - First part complete, Second part (2D) hardware setup & testing done
M3 - Apr05 - Second part done

Contingency plans
We expect the most difficult parts of the project to be the detecting of the ball’s xy-coordinates on the surface (as no simple sensor will be able to accomplish this) and designing a mechanical structure that can precisely control the direction of the surface’s slope (as the interaction of two servo motors can introduce large errors). As a result, a scaled-down version of the project will be attempted first as described in the Overview. As the scaled-down version will only have one degree of freedom and one simple ultrasonic sensor, the risk of failure will be low.

