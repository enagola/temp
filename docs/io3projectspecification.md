---
title: Project Specification
layout: template
filename: io3projectspecification
pageheader: page-header-specification
--- 

# Project Charter

## Project Overview

Our project, the robot known as RD-1, is a self balancing robot that has the goal of assisting oureveryday retrieval needs.  The goal of the project is to have RD-1 be able to listen to commandsfrom people similar to that of google, siri, and alexa, and be able to interpret that command in orderto complete a task.   Some general tasks that the robot will be able to do is interact with a user,recognize objects, move on its own, and be aware of its overall surroundings.  With these generaltasks the robot will be able to take simple commands of retrieval, locate objects that were requestedand move to those object.  After being able to do that, the robot will expand towards being able topick up those objects, locate the person who requested it, and bring the object to them.

## Project Approach

Our approach towards this project is to use the pre-existing self-balancing robot,  ELEGOO, andhook it up to cameras, speakers, and other listening devices to create the robot’s ‘eyes, ears, andmouth’.  In addition, we are going to use the adruino to balance the robot and a raspberry pi forboth the voice and object recognition.  We plan on using tools like python software, Arduino IDE,and voice recognition libraries to code a machine learning algorithm that uses computer vision suchas OpenCV and voice recognition similar to google, siri, and Alexa as well as neural networks tolearn and adapt to its environment.  With this software we hope to accomplish the robot’s abilityto rotate its camera and move around on its own, recognize objects that it’s camera picks up as itmoves around, be able to turn speech into words it can understand, and be able to execute simplecommands from those words.

## Minimum Viable Product

The minimum viable product that we hope to achieve is for our robot to be able to recognize voice speech, be able to rotate its camera, and be able to recognize objects correctly. The goal for this minimum viable product is to be reached within the next month. This specification of the minimal viable product is important because of the crucial basic functionality that it demonstrates needed for the further development goals that follow. Specifically, to achieve this minimum viable product we will start by simply connecting the robot to the cameras and the raspberry pi and testing out basic robot movement and send the images of what the robot sees to our computer. Then we will connect the robot’s speaker and create simple commands that show us that the robot is able to produce speech.

After this we plan on trying to create the computer vision for the robot and testing if the robot is identifying the labels of what it sees correctly possibly by having the robot speak about what it sees. Following this, we will probably focus on the movement of the robot teaching the robot to turn its head and move around. Then we will focus on the robots 'ears’, testing if the robot, when asked to do so, can recognize our speech and maybe ask the robot to read out what it understood from our speech. At that point, the robot should be at a point where it has all of the basic functionality needed to adjust them to the ultimate goal.

As we have time we would add on features that connect the voice recognition to the object recognition by having the robot recognize simple commands like “locate the cup” while the robot is facing in front of a cup. After this we can connect it further to the movement of the robot by having it try to execute the locate command with the robot understanding that the object can be anywhere in it’s 360 degree radius.

If this all works and we have more time, we would want the robot to start moving towards the object giving the robot spatial awareness. Up to this point, we are being ambitious but believe that this could be the end goal of the quarter. Past this quarter, we would hope to give the robot the ability to pick up objects in order to fully implement the retrieval aspect. Furthermore, another long term goal would be to have the robot be able to move around and have a greater awareness of location of objects. For example, instead of just rotating in order to find an object, the robot would be able to move around into different areas as it is rotating to cover a larger space when trying to detect the object requested.

## Constraints, Risk, and Feasibility

### Constraints

This is a quarter-long project, so everything needs to be completed in a short period of time, so wecan leave a little room for debugging or hardware issues that we might encounter with the robot.Voice Recognition module can recognize and execute human’s command will be the lengthiest partof our project so most of our time and debugging might be spend trying to implement that.Robot can go to the target, avoid obstacles on the way and come back to the start point.

### Risks

We need to handle everything virtually, so it is easy to get unconnected and unsynchronized witheach other.Software such as the Python built-in libraries and packages might not work as expected with thegoal that we are trying to achieve.Voice Recognition module is hard to implement in Google Voice Recognition APICamera might not capture all the objects in the room, so it needs to be in the sensor’s range

### Feasibility

Balancing robot is already implemented with small error.  Voice recognition can be executed withsome easy commands.  Object detection part is supported by Python library, so this part will needto have an improvement. The robot being able to listen to a person command and executing itcan be done using python speech recognition libraries and further improving it so that the robot canbetter understand commands. Making the robot execute the commands can be done by specifyingthe format that a should be said so that it can be filtered and the robot knows where to go and what object it needs to get.

# Group Management

The major roles in our groups management is that Ninh Tran is the head of the technical side of theproject while Ethan Nagola is the head of the logistics. All of us will be working interconnectedly but, as of now, Ninh Tran and Khanh Pham will have a larger role in the voice recognition software and Ethan Nagola and Andres Bernal will play a larger role in the computer vision and movementaspects. Overall decisions will try to be made by unanimous consensus but if there is a disagreement then those who are more in charge of the area involved will have a larger say in the matter.  Wewill communicate both through zoom and through discord asking questions and meeting up whennecessary. We will try and keep on schedule and Ethan Nagola will try and manage the plan to makesure this happens by being conscious of everyone’s schedules.However, if we fall behind we willfocus on what is most important to get the most of the work that we do.

# Project Development

In our project to make an intelligent droid, we develop both hardware and software for it.  In the limit time of 10-week, We don’t build this droid from scratch.  We bought all the mechanical body parts such as frames, motors, and wheel from ELEGOO (<https://www.elegoo.com/pages/arduino-kits-support-files>).   We  also  purchased  the  fundamental  control  boards  such  as  Arduino,  sensorboard, and motor driver. Adding all these components, we could save time to have a basic droid.We decide to use Arduino Uno to control all the mechanical parts and read basic sensors  tomake this droid  stand  balance.Raspberry pi charges for all intelligent functions such as objectrecognition, voice recognition, finding the path. Raspberry pi connects with Arduino Uno via USBcable to send and receive commands.  Currently, we have all the needed hardware parts, ArduinoUno, and all kinds of sensors, Raspberry pi, camera, speaker, microphone, robot assembly parts.

# Project Milestones and Schedule

The original schedule for the project, and the proposed milestones go throughout the project and how the milestones will complete.

| week | Type      | Description                                                                                                                                                                                                   | Dev  |
|------|-----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| 4    | Milestone | Build a self-balance robot from its parts, including mo-tors, aluminum alloy boards, motor brackets, couplings,footholds, circuit control board (Arduino Nano), sensorboards, battery box, ultrasonic sensor. | Ninh |
|      | Milestone | Update the Raspberry Pi to the top.  Connect RaspberryPi to Arduino Nano via USB. Test the robot and adjustthe balance. | Ninh |
|      | Milestone | Report project specification. | Ninh, Khanh, Andres, Ethan |
|      | Milestone | Project web presence on Github. | Andres, Khanh|
| 5    | Milestone |Update the Github repo to website | Andres, Khanh|
|      | Milestone |Familiar with gTTS(text to speech) and Deepspeech(Speech To Text) | Ethan, Andres|
|      | Milestone |Familiar with TensorFlow Object Detection AP on Rasperry pi | Ninh, Khanh|
| 6    | Milestone |Implement python code to detect objects| Ethan, Andres|
|      | Milestone |Implement python code to speak and hear | Ninh, Khanh|
| 7    | Milestone |Detect objects, interact with a human, receive the voicecommand. The droid finds an object depending on the order | Ninh, Khanh|
|      | Milestone |Develop website to control and monitor the droid  | Ethan, Andres, Ninh|
| 8    | Milestone |Detect objects, interact with a human, receive the voice command. The droid finds an object depending on the order(continue) | Ninh, Khanh|
|      | Milestone |Develop website to control and monitor the droid (continue). | Ethan, Andres, Ninh|
| 9    | Deliverable |Optimize code, adjust the droid to reach the goal | Ethan, Andres, Khanh, Ninh|
| 10   | Deliverable |Final report and video | Ninh, Khanh|
|      | Deliverable |Final report and video| Andres, Ethan|
|      | Deliverable |Update the website | Ethan, Andres, Khanh, Ninh|

# Individual's Tasks

## Week 4

### Ninh

| Description | Build a self-balance robot from parts |
|-------------|---------------------------------------|
|             | Use all parts usach as motors, aluminum alloy boards, motor brackets, couplings, footholds, circuit control board (Arduino Nano), sensor boards, battery box ultrasonic sensor to make a droid                       |
|  | Update the Raspberry Pi to the top. Connect Raspberry Pi to Arduino |
|  | Distribute tasks and create project milestones and schedules for the team.|
| Completion Criteria: | The droid can stand self-balance and move. Schedule the project, including the proposed milestones.|

### Ethan

| Description          | Report project specification                                                                    |
|----------------------|-------------------------------------------------------------------------------------------------|
|                      | Work with part 1 and part 2 of project specification. Revise all parts of project specification |
| Completion Criteria: | Finish all the requirements for project specification                                           |

### Khanh & Andres

| Description | Project web presence on Github                          |
|-------------|---------------------------------------------------------|
|             | Build the GitHub repository for for project web presence|
|Completion Criteria:| Finish the basics requirements for project web presence|

## Week 5

### Khanh & Andres

| Description | Update the Github repo to website|
|-------------|-------------------------------------------------------|
|             | Base on GitHub pages to build a website for project web presence|
|Completion Criteria:| The website contains Project Specification, images,videos.|

### Ethan & Andres

| Description | Familiar with TensorFlow Object Detection AP on Raspberry pi|
|-------------|---------------------------------------|
|Completion Criteria:| Install and TensorFlow Object Detection AP on Raspberry pi, detect some simple objects.|

### Ninh & Khanh

| Description | Familiar with gTTS( Text To Speech) and Deepspeech (Speech To Text)|
|-------------|---------------------------------------|
|Completion Criteria:| Install gTTS( Text To Speech) and Deepspeech (Speech To Text), work with some basics commands.|

## Week 6

### Ethan & Andres

| Description |Implement python code to detect objects and computer vision|
|-------------|---------------------------------------|
|Completion Criteria:| Detect some objects, return the labels, and locate these objects. The droid should understand all kinds of things
around it.|

### Ninh & Khanh

| Description | Implement python code for voice recognition from human and droid’s voices( speaker)|
|-------------|---------------------------------------|
|Completion Criteria:| Using Deepspeech (Speech To Text), the droid understands human commands. Droid use gTTS( Text To Speech) to talk with human.|

## Week 7,8

### Ninh & Khanh

| Description |Detect objects, interact with a human, receive the voice command. The droid finds an object depending on the order|
|-------------|---------------------------------------|
|Completion Criteria:| The droid could do some intelligent tasks.|

### Ethan, Andres & Ninh

| Description | Develop website to control and monitor the droid|
|-------------|---------------------------------------|
|Completion Criteria:| Control and view the environment around the droid.|

## Week 9

### Ethan, Andres, Ninh & Khanh

| Description |Optimize code, adjust the droid to reach the goal.|
|-------------|---------------------------------------|
|Completion Criteria:| The droid could do some intelligent tasks.|

## Week 10

### Ninh & Khanh

| Description | Final report and video.|
|-------------|---------------------------------------|
|Completion Criteria:| Finish all the tasks.|