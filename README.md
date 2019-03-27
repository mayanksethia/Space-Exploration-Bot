# Space-Exploration-Bot

Main Idea: 
We plan to build an prototype of a smart bot whose architecture would be similar to which can solve the problem easily. Sensors like ultrasonic sensors would be used to detect obstacles to draw an entire map of the range. Humidity and temperature sensor and magnetic field sensor will give us an update about the surroundings conditions based on which an analysis can be drawn on how is the environment condition.

Technology Stack

Raspberry PI will the main controller of the bot which will take the data from the base station given by the operator. Two arduino UNO will be attached to the bot to carry out the various functionalities. The first arduino will basically monitor the controlling of the bot along with an ultrasonic sensor attached to the mapping of an entire place. An L293D motor driver is also attached to the bot to control the motors according to the movement instruction. Using the same mapping the data the bot will then traverse autonomously. It will send the mapping data back to raspberry Pi which will send the data back to base station and will be displayed on a GUI. The other Arduino will control the robotic arm movement of the bot. The arm will be basically attached to a PWM motor driver to control the servo motors. This arm can be used to retrieve objects and research particles like soil, stone, fluids and other stationary objects. The arm will be semi-autonomous and will be controlled using the user at the base station. And the data would flow through the R pi to the arduino. This arduino will also have a sensors attached to it like gas sensors, humidity sensors, magnetometer to carry out the analysis of properties of the area. There will be a camera attached to the bot to give live video feed which can be again viewed on the base station and can be used to carry out image processing.

Implementation: 
First we use PyCDA(An Image Processing module) to detect craters from the Satellite images of surface. The x,y and diameter of the craters are then found out by running the code in the file testing1.py. The coordinates thus optained are then put as input to the RRT algorithm which we use to determine the paths between two points such that it does not fall into the craters. The code for this file is in path.py

Screenshots for the swarm robotics implementation using the UnReal Engine is also added with the names op1 and op2. '

Taking the sensor values from the various sensors we are passing it to the AR console Unity, where we are using Augmented Reality to show the same in RealTime as a DashBoard. 
