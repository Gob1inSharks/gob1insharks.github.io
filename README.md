# Intelligent Trolleys

Jayden Chen.
November 19th, 2022.

![shanghaiyaya](/assets/photos/trolly.jpg "shanghaihighway")

## 1. Introduction

### 1.1 Background

Traveling internationally is always a problem for many, especially in airports. Families bring large amounts of luggage, and it could be difficult pushing the luggage trolley(s) around a busy airport with crouds of people. Many people find airport trollies hard to control, especially with luggage on them.

What if there was a way to move trollies around with ease?

![airportlugaggetrolly](/assets/photos/Lugaggetrolley.jpg "generictrolley") 

Demostration of a trolley. Source from Getty Images.

With this in mind, I plan to create an intelligent trolley that could follow the user's directions. There should be a camera that detects where the user is, and the user should be able to direct the trolley anywhere without a remote controller. 

### 1.2 Objective

How can I create a camera controlled trolley that improves travelling through airports?

### 1.3 Initial Ideas

![sketches1](/assets/photos/IntelligentTrollySketches.png "sketches1")

Intial Sketches I've Creating (Using Adobe Illustrator) of the intelligent trolly.

![sketches2](/assets/photos/IntelligentTrollyProject.png "flowchartsketch")

Flow chart of the entire project. 

## 2. Mthodology

### 2.1 Overview





### 2.2 Hand Detection

To 

For better control of the vehicle, I used a camera to scan images of my hands. 
Using hand detection. This allows me to guide the car to any direction with ease. It is a quick, easy way to give understandable inputs to the system.

Mediapipe is a framework for building machine learning pipe lines to process video and audio. I use Mediapipe Hands to detect the direction in which my point is pointing to.

![hand_graph_2](/assets/photos/mediapipe_hand_photo.png "hand_graph_2")
![hand_graph](/assets/photos/hand_landmarks.png "hand_graph")

The above models shows the coordinates of the hands that mediapipe maps out. Photo from [Mediapipe Development Site](https://google.github.io/mediapipe/solutions/hands.html "Mediapipe Solution: Hands").

### 2.3 Three-Dimensional Simulation

To better understand how the vehicle is moving, there should be a virtual simulation of the car. This way, the drivers understand how the vehicle moves better and could manage to remote control them.

![codeforvtk](/assets/photos/"code1024.jpg" "code1024")

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

I finished building the pre-designed mecanum wheel in a day, to test out how a mecanum wheel vehicle moves.

![V1](/assets/photos/vehicle_demostration.jpg "VD1")
![V2](/assets/photos/vehicle_demostration_2.jpg "VD2")
![V3](/assets/photos/vehicle_demostration_3.jpg "VD3")

Above are photos of the vehicle.

### 4.3 Design Process (5th - N week)

Have no finished yet.

### 4.4 Final Product (N week)



## 5. Reflection

### 5.1 Conclusion



### 5.2 Improvements



### 5.3 Take Aways






