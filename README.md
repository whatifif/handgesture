[Home](/README.md) | [Gestures](/gestures.md) | [Reference](/reference.md) | [Edit Guide](/editguide.md) | <button class="nav" ><a href="https://github.com/whatifif/handgesture/">View on Github</a></button>  |  <button class="nav" ><a href="https://whatifif.github.io/handgesture/">View on Web</a></button>

[draft-d](/draft-d/README.md) | [draft-h](/draft-h/README.md) | [draft-j](/draft-j/README.md)

# Controlling a Computer by Hand Gesture

## TODOs

1. ### getting more data of hand gesture.

2. ### connecting a trained model 
   a. making the model recognise a gesture in application program ( stream-lined at real time)

3. ### making a demo program
   a. calculation program
   
   b. running dinosaur ?
  
4. ### preparing a presentation
   a. introduction
   
   b. creating data sets
   
   c. training and testing
   
   d. demo
   
   e. summary and future work
   

5. ### tracking a right hand for mouse ?

## Brief Introduction of the project of Team Echo

Almost people use a desktop or laptop these days. One of serious problem is that we are stuck to the keyboard and mouse, which will cause a serious health problem on a long run. Moreover in VR/AR age, we cannot use keyboard/mouse. Our purpose is to replace a keyboard and mouse with hand gestures. We have devised a virtual keyboard and virtual mouse with subtle hand gestures and made ML recognise our gestures so that we can control our computer remotely. Amazon echo has ear now. It will have eye in future. We need to make a standard gestures for people to adopt easily like a standard keyboard and mouse. ML will address this for us, human. We used Deep Learning as ML in this project.


## Introduction

People have used a keyboard and mouse as a standard way of input to computer for a long time. One of the serious problem of using keyboard and mouse is that we are stuck to the keyboard/mouse and sit still while we are using our desktop or laptop computer. This causes a serious health problem on a long run. 

Moreover we are entering the VR ( Virtual reality )/ AR ( Augmented reality ) age and we cannot use keyboard/mouse as we did before. We have to use some kind of mobile controller or GESTURE !!!

ML( Machine Learning ) can recognise our gesture and control the computer as we intented by gesture remotely.
We will feel like a magician. And by moving our body to control the computer, we can avoid sitting still and getting a health problem. Moreover we can play a game with much more immersive experience by moving our hands, heads and body.

To replace a keyboard and mouse, we have to devise many subtle gestures and these gestures have to be easy one for people to learn easily like a standard keyboard and mouse. It may be annoying if we have to learn different gestures to control different devices in future.

We suggest a standard virtual keyboard and standard virtual mouse like following. The goal of this project is to search a possibility of using these subtle gestures to control a computer up to the level to replace a keyboard and mouse completely.


## Recent works in this field

1. [Carnegie Mellon University OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose): webcam

2. [Microsoft hololens](https://www.microsoft.com/en-au/hololens): 3D sensor

3. [Microsoft hand tracking](https://www.microsoft.com/en-us/research/project/fully-articulated-hand-tracking/): 3D sensor

4. [Leap Motion](https://www.leapmotion.com): 3D sensor

5. [Mano Motion](https://www.manomotion.com/): smartphone camera

6. [PilotBit Mobile Hand Tracking](http://www.pilotbit.com/): 3D sensor


## Challenging points

1. using a webcam without using 3D sensor (depth camera)

2. detecting the subtle gestures at real time

3. deep learning running at mobile devices such as smartphone, smartglasses and VR/AR headset


## Work flow

1. defining as many hand gestures as possible to cover all the keys on a keyboard.

2. creating many data sets accordingly.

3. searching for a deep learning model which can track and recognise these hand gestures at real time.

4. coding for hand gesture recognition

5. coding for hand tracking

6. creating some demos such as basic calculation or a game.

## Tools used for Team work
[github site for project page](https://github.com/whatifif/handgesture)
[github site for coding work ](https://github.com/whatifif/handgesturecode)
[ slack, https://sml109.slack.com](https://sml109.slack.com) for team communication and instant file sharing

## Hardwares
1. Coding with MacBook Air (i7, 8GB RAM)
2. ML Model training with nvidia GTX 960 (2GB Graphic memory) on i7 CPU, 8GB RAM, ubunutu 14.04 64bit personal computer

## Why MxNet?


## How can the trained model be transferred to work at smartphone?


## Is the detection area ( Region of Interest ) for hand needed?




### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/whatifif/handgesture/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.

### [LICENSE](/LICENSE)
GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007

Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
 
 Everyone is permitted to copy and distribute verbatim copies
 of this license document, but changing it is not allowed.
