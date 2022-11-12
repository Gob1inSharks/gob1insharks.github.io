# Utilizing Mediapipe to Control an Omnidirectional Vehicle

Jayden Chen,
November 12th, 2022.

## 1. Introduction

### 1.1 Background

There are a lot of problems with modern urban infrastructure. With cars dominating the roads, accidents happen frequently which result in loss of time, resources, and sometimes even lives. Could there be a solution to this problem? Are trucks and human drivers the most reliable resource? 

I believe that omnidirectional vehicles with remote control can be a viable replacement.

For this project, I plan to make a small model of what could be a future vehicle for transportation.

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

The above models shows the coordinates of the hands that mediapipe maps out. Photo from [Mediapipe Development Site](https://google.github.io/mediapipe/solutions/hands.html "Mediapipe Solution: Hands").

### 2.3 Three-Dimensional Simulation

To better understand how the vehicle is moving, there should be a virtual simulation of the car. This way, the drivers understand how the vehicle moves better and could manage to remote control them.

![codeforvtk](/assets/photos/"WeChat Image_20221112153028.jpg" "code1024")

### 2.4 Mecanum Wheel Vehicle

Mecanum wheels are omnidirectional wheels or wheels that can move in right-left and forward-backwards motion. With a special shape, the wheels allow my vehicle to move in any direction. An advantage of mecanum wheels is that they can directly replace the normal four wheel drive. This could be a great option for my vehicle.

![mecanum_wheel_graph](/assets/photos/Mecanum_wheel_control_principle.svg.png "mwg02")
![mecanum_wheel_graph2](/assets/photos/graph_mecanumwheels.png "mvg01")

The above graphs shows how mecanum wheels work.

![uranus](/assets/photos/UranusOmniDirectionalRobotPodnar.png "uranushaha")

Here is an example of a mecanum wheel vehicle. "URANUS" omni-directional mobile robot using Mecanum wheels. Designed in 1985 by Gregg Podnar at the Robotics Institute of Carnegie-Mellon University. Sources from [Wikipedia Page for Mecanum Wheel](https://en.wikipedia.org/wiki/Mecanum_wheel "WikitheCan").

### 2.5 System

### Mediapipe

Utilizing mediapipe, I was able to create python program where the direction I am pointing in through the camera. 

### VTK

VTK or Visualization Toolkit is a powerful open-source software to display visual infomation. In the python program, I have included a vtk simulation of the vehicle.

### Serial COM

The vehicle is connected to the laptop using a serial COM, allowing communication between the program and the vehicle.

### Vehicle

Luckly enough, I did not have to design a mecanum wheel vehicle. There was a mecanum vehicel using Arduino Uno that I had to assemble. 

## 3. Results

### 3.1 Overview

Have no finished yet.

## 4. Process

### 4.1 Learning Process (1st - 3rd week)

The processed beginned with me learning how to use VTK to make a simulation. I already knew python and mediapipe so the process was fast. 

![VTK](/assets/photos/VTK_learning_demostration.jpg "VTK_demostration")

Above is a photo of code I worked on.

### 4.2 Building Process (4th week)

I finished building the pre-designed mecanum wheel in a day.

![V1](/assets/photos/vehicle_demostration.jpg "VD1")
![V2](/assets/photos/vehicle_demostration_2.jpg "VD2")
![V3](/assets/photos/vehicle_demostration_3.jpg "VD3")

Above are photos of the vehicle.

### 4.3 Design Process (5th - N week)

Have no finished yet.

### 4.4 Final Product (N week)

Have not finished yet.

## 5. Reflection

### 5.1 Conclusion

With further developments in self-driving cars, it seems important to rethink how the roads and vehicle of cities work. It is important to keep all possibilities in mind, so that we can find more efficient and safe ways for transportation. 

### 5.2 Improvements

I think the hand detection system could have been enhance. Mediapipe is a great resource, yet it could only impliment a 2d surface. The user interface with the program isn't well-designed and it is an aspect tht can be greatly improved upon. Maybe I'll revisit this project in the future and improve it.

### 5.3 Take Aways

Overall, this project went smoothly. It wasn't a big project, yet I manage to complete all of my goals. 

In this project, I have learned how to use VTK. VTK is definitely a tool that I will be using in the future for its display of visual infomation. Further more, learning how to create a portfolio online is vital for future projects, and this is thefirst project I applied that to. 




