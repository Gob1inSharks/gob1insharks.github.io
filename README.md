# Utilizing Mediapipe to Control an Omnidirectional Vehicle

## 1. Introduction

### 1.1 Background

There are a lot of problems with modern urban infrastructure. With cars dominating the roads, accidents happen frequently which result in loss of time, resources, and sometimes even lives. Could there be a solution to this problem? Are trucks and human drivers the most reliable resource? 

I believe that omnidirectional vehicles with remote control can be a viable replacement.

![shanghaiyaya](/assets/photos/elevated-view-of-shanghai-highway-weiyi-zhu-3643787103.jpg "shanghaihighway")

### 1.2 Objective

How can I utilize camera to control an omnidirectional vehicle in both physical and simulation form?

## 2. Mthodology

### 2.1 Overview

The project is composed of one input and two outputs. The input being Mediapipe hands; the ouputs being the vehicle and its simulation. Using mediapipe, my laptop can get the direction of my hand(s). The car then moves to the direction my hand(s) is pointing at. There is also a VTK simulation of the car running alongside the physical one. The vehicle is connected to my laptop with a serial port, while the rest is in a python program. 

### 2.2 Hand Detection

For better control of the vehicle, I used a camera to scan images of my handsUsing hand detection. This allows me to guide the car to any direction with ease. It is a quick, easy way to give understandable inputs to the system.

Mediapipe is a framework for building machine learning pipe lines to process video and audio. I use Mediapipe Hands to detect the direction in which my point is pointing to.

![hand_graph_2](/assets/photos/mediapipe_hand_photo.png "hand_graph_2")
![hand_graph](/assets/photos/hand_landmarks.png "hand_graph")

The above model shows the coordinates of the hands that mediapipe maps out. Photo from [Mediapipe Development Site](https://google.github.io/mediapipe/solutions/hands.html "Mediapipe Solution: Hands").

### 2.3 Three-Dimensional Simulation

To better understand how the vehicle is moving, there should be a virtual simulation of the car. This way, the driver is understand how the vehicle moves.

### 2.4 Mecanum Wheel Vehicle

Mecanum wheels are omnidirectional wheels or wheels that can move in right-left and forward-backwards motion. With a special shape, the wheels allow my vehicle to move in any direction. An advantage of mecanum wheels is that they can directly replace the normal four wheel drive. This could be a great option for my vehicle.

![mecanum_wheel_graph](/assets/photos/Mecanum_wheel_control_principle.svg.png "mwg02")
![mecanum_wheel_graph2](/assets/photos/graph_mecanumwheels.png "mvg01")
The above graphs shows how mecanum wheels work.

![uranus](/assets/photos/UranusOmniDirectionalRobotPodnar.png "uranushaha")

Here is an example of a mecanum wheel vehicle. "URANUS" omni-directional mobile robot using Mecanum wheels. Designed in 1985 by Gregg Podnar at the Robotics Institute of Carnegie-Mellon University. Sources from [wikipediapageformecanumwheels](https://en.wikipedia.org/wiki/Mecanum_wheel "WikitheCan").

### 2.5 System

### Mediapipe

Utilizing mediapipe, I was able to create python program where the direction I am pointing in through the camera. 

### VTK

VTK or Visualization Toolkit is a powerful open-source software to display visual infomation. In the python program, I have included a vtk simulation of the vehicle.

### Serial COM

### Vehicle

## 3. Results

### 3.1 Overview

## 4. Process

### 4.1 Learning Process

### 4.2 Building Process

### 4.3 Design Process

### 4.4 Final Product

## 5. Reflection

### 5.1 Overview

### 5.2 Improvements

### 5.3 Take Aways

### 5.4 Conclusion
