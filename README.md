[Home](/README.md) | [Gestures](/gestures.md) | [Blue_Background](/blue_background.md) | [Reference](/reference.md) | [Edit Guide](/editguide.md) | <button class="nav" ><a href="https://github.com/whatifif/handgesture/">View on Github</a></button>  |  <button class="nav" ><a href="https://whatifif.github.io/handgesture/">View on Web</a></button> | [Teams-all](/teams-all/SML109_team_project_abstracts.pdf)


# Controlling a Computer by Hand Gesture

## Study group of Sydney Machine Learning

This study group is formed to study the [Harvard CS109](https://github.com/cs109) among the members of [Sydney Machine Learning Meetup](https://www.meetup.com/Sydney-Machine-Learning/). 

Members were re-grouped into 10 teams and completed their own interesting projects. 
 My team was "team echo" named after the prize Amazon Echo.

- study period: 2017.08.02 ~ 2017.10.23 ( 3 months including 1 month project )
- study place : Amazon Web Service ( [https://aws.amazon.com/](https://aws.amazon.com/), Australia, 2 Park St, Sydney NSW 2000 )

## Project

- name: Controlling a Computer by Hand Gesture  
- homepage: [https://github.com/whatifif/handgesture](https://github.com/whatifif/handgesture)  
- code page: [https://github.com/whatifif/handgesturecode](https://github.com/whatifif/handgesturecode)  
- slack: [https://sml109.slack.com](https://sml109.slack.com)  
- team name: Team Echo 
- team members: heeseob, jiaxi
- period: 1 month

Among 10 teams, we got the 1st prize ( and Amazon Echo ( Alexa ) as a award ) along with one other team ( DeepAI ).

## Brief Introduction of this project

Almost people use a desktop or laptop these days. One of serious problem is that we are stuck to the keyboard and mouse, which will cause a serious health problem on a long run. Moreover in VR/AR age, we cannot use keyboard/mouse. Our purpose is to replace a keyboard and mouse with hand gestures. We have devised a virtual keyboard and virtual mouse with subtle hand gestures and made ML recognise our gestures so that we can control our computer remotely. Amazon echo has ear now. It will have eye in future. We need to make a standard gestures for people to adopt easily like a standard keyboard and mouse. ML will address this for us, human. We used Deep Learning as ML in this project.

- Using hand movements and gesture to control mouse/clicks though cam  
![Control-Your-Home-With-Gesture-And-Voice-Using-Flowton](/resources/remote-control800x.jpg)


## Introduction

People have used a keyboard and mouse as a standard way of input to computer for a long time. One of the serious problem of using keyboard and mouse is that we are stuck to the keyboard/mouse and sit still while we are using our desktop or laptop computer. This causes a serious health problem on a long run. 

Moreover we are entering the VR ( Virtual reality )/ AR ( Augmented reality ) age and we cannot use keyboard/mouse as we did before. We have to use some kind of mobile controller or GESTURE !!!

ML( Machine Learning ) can recognise our gesture and control the computer as we intented by gesture remotely.
We will feel like a magician. And by moving our body to control the computer, we can avoid sitting still and getting a health problem. Moreover we can play a game with much more immersive experience by moving our hands, heads and body.

To replace a keyboard and mouse, we have to devise many subtle gestures and these gestures have to be easy one for people to learn easily. And these gestures should be a standard like a standard keyboard and mouse. It may be annoying if we have to learn different gestures to control different devices in future.

We suggest a standard hand gestures like follows. The goal of this project is to search a possibility of using these subtle hand gestures to control a computer up to the level to replace a keyboard and mouse completely.


## Recent works in this field

1. [Carnegie Mellon University OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose): webcam

2. [Microsoft hololens](https://www.microsoft.com/en-au/hololens): 3D sensor

3. [Microsoft hand tracking](https://www.microsoft.com/en-us/research/project/fully-articulated-hand-tracking/): 3D sensor

4. [Leap Motion](https://www.leapmotion.com): 3D sensor

5. [Mano Motion](https://www.manomotion.com/): smartphone camera

6. [PilotBit Mobile Hand Tracking](http://www.pilotbit.com/): 3D sensor


## Challenging points

- using a webcam without using 3D sensor (depth camera)

- detecting the subtle gestures at real time

- deep learning running at mobile devices such as smartphone, smartglasses and VR/AR headset



## Work flow

1. searching github for open sources and youtube for useful information.

2. defining as many hand gestures as possible to cover all the keys on a keyboard and mouse.

3. coding for tools to create as many data sets as possible in short time.

4. coding to use a deep learning model which can recognise these hand gestures at real time.

5. coding for tracking and capturing hand

6. coding for some demos such as basic calculation or a game.



## Tools used for Team work
1. github site for project page: [https://github.com/whatifif/handgesture](https://github.com/whatifif/handgesture)  
2. github site for coding work : [https://github.com/whatifif/handgesturecode](https://github.com/whatifif/handgesturecode)  
3. slack for team communication and instant file sharing: [https://sml109.slack.com](https://sml109.slack.com)   

## Technical Details

#### Main Dependencies:
 - Python 2.7
 - Opencv 3.2.0
 - MxNet 0.11.0
 - Numpy 1.13.1
 - Pandas 0.20.3

#### Hardwares and softwares
 - Coding with MacBook Air (i7, 8GB RAM)
 - ML Model training with nvidia GTX 960 (2GB Graphic memory) on i7 CPU, 8GB RAM, ubunutu 14.04 64bit personal computer
 - Microsoft Webcam HD-3000
 - MacBook Air webcam
 - jupyter notebook as python editor


## Hand Gestures as a Standard Way of Input like a Keyboard and a Mouse
- Using hand for a future virtual keyboard
![virtual keyboard](/resources/virtual-keyboard2.jpg)  

We have two hands normally. We can use one hand for keyboard and the other for a mouse.
The standard gestures should be easy for people to learn easily. Just imagine that there is a virtual keyboard in front of your left side and virtual mouse on your right side. Lets focus on virtual keyboard first.

We divided the left side into three regions

1. left region
2. middle region
3. right region

- left, middle and right region of the left side.  
( Thses are LEFT side images. Images are flipped horizontally when captured. So do not be confused )    
![left middle right region of left side](/resources/gestures/l-m-r.png)


We can make 10 easy distinct gestures on each region:

1. closed hand
2. open hand
3. thumb only
4. additional index finger
5. additional middle finger
6. folding first finger
7. folding second finger
8. folding middle finger
9. folding index finger
10. folding thumb

If we use 6, 7, 8, 9, 10 as inputs, we have 5 * 3 = 15 different gestures in each region and 15 * 3 = 45 gestures in total region.

If we use 3, 4, 5 as control, we have 3 * 3 = 9 controls and 45 * 9 = 135 different gestures which will cover the whole range of keys ( numbers, lower alphabets, upper alphabets, special keys and controls )

For a right hand as a mouse, we can have 10 same gestures as left hand, which cover whole inputs from mouse. Our center of hand is a mouse cursor. The mouse cursor of computer will track the center of the right hand. There is only one region on the right side for a mouse.

For a left-handed people, of course we can swap the left with the right.

- 30 hand gestures suggested as a standard way of input for remotely-controlled devices.
![hand gestures](/resources/gestures/hand_gestures.png)
  
  [See the detailed gestures for keyboard and mouse](/gestures.md)

## Making a data set
To train the ML, several thousand data are needed and these data are to be prepared by ourselves.
So we have to make a program for capturing the hand images easily. With the capturing program, about 2000 hand images were captured in short period.

## Detecting and tracking Hand
Since we are moving our hands freely in front of webcam, our hands should be detected and tracked correctly in the frame of webcam image at real time. Haar cascade, background substraction and skin color detection were tried to track a hand. Skin color detection was found to be stable.

#### detection region for hand and mouse
Since our face has a same skin color as our hands, we have to find ways to ignore the face. Haar cascade can be applied for this purpose. But due to the time limitation of this project, we simply defined a detection region and tried not to push our face into that region.  

![See the blue_background used to capture hand images](/blue_background.md)


#### tracking hands
Since we use a skin color for tracking a hand, background color and our shirts color should be a contrasting color to skin color. And we have to wear a long sleeve shirt to hide our arm from detection also.

The environment light affects skin color significantly. So bright room was avoided. And a blue screen made with blue color table cloth was used as a background to get a good data. It turns out that the whiteboard is a good background also.

- Main program used to capture hand images:  
There are two detection regions. When the buttons below are clicked, detected image is captured, resized into 200x200 and saved in jpg format. At the same time, the file name is saved in csv file also. 2000 data were obtained in short period.  
![tracking hands](/resources/tracking_hands800x.jpg)

# Deep Learning Model to recognise the gesture

## Difficulties
 - Very few existing dataset fits our purpose. Therefore, we have to capture the hand picture, and do the labeling. A.k.a, we will have to make the dataset our own

 - Tracking and recognizing hand are 2 challenges in this project, and each requires large amount of time to work on. Therefore, in this project, we are firstly focusing on Recognition, and used a just feasible approach for Hand Detection for saving time. 

 - Model selections, especially on building a Neural Nework architecture. That is, if the Neural Network is too "deep", it takes long time to converge, and also is not suitable in real-time cameras. While single-layer NN does not performing good enough
 
 - 200x200 pixel image data in jpg format gets "out of memory" error when Nvidia GTX 960 ( 2GB Graphic memory) is used for training a Deep Learning Model. So 64x64 version of data are prepared and used to train a Model.
 
 - There are intermediate gestures between any two gestures while capturing at real time. If ML is forced to continuously predict these intermediate gestures, ML will make much mistakes. We had to capture only 1 out of 10 frames and only if the 3 consecutive predictions are same, we took the gesture as a final gesture. So the delay shown on demo is not the actual delay due to ML processing. 

## Why MxNet is chosen as a Deep Learning Model of this project?
- Super fast
- Various language bindings: R, Python, Scala, Perl, Julia
- Strong API interface
- Scale linearly and easily
- Easy to deploy into production


## How can the trained model be transferred to work at mobile devices such as smartphone?
Two ways:

1. The trained model can be install onto the smartphone, and does the prediction in the client side. In this case, the model needs to be periodically updated, and might require a large update pacakage of the application

![](https://github.com/whatifif/handgesture/blob/master/draft-j/resources/client.png)

2. The trained model stays at the application server, while keeping the detection utility and necessary preprocessing in the client side to reduce the workload overhead on the server. Therefore, the model can be periodically updated without impact on the client application much.  

![](https://github.com/whatifif/handgesture/blob/master/draft-j/resources/server.png)


### Main Work Flow:

![](https://github.com/whatifif/handgesture/blob/master/draft-j/resources/workflow.png)

### Model Details

 - ~1800 images for training
 - ~200 images for testing
 - Mini-batch size 128
 - Model converge around 400 iterations, with Learning Rate 0.001
 - Weight decay set to 0.001 for regularize the model for overfitting
 - Achieved over 97% accuracy on evaluating test dataset

    ![](https://github.com/whatifif/handgesture/blob/master/draft-j/resources/learning_curve.png)


## Summary of Progress

- The possibility to use subtle hand gestures for controlling a computer remotely is confirmed.

- A standard hand gestures for people to learn easily and replace a whole keyboard and mouse is suggested.

- Left hand is used for keyboard, Right hand is used for mouse, which can be swapped for left-handed people

- Left hand can have 30 gestures based on the hand gesture, and their angles in the picture. This 30 gestures can be mapped to 135 different keys in the keyboard.




## Demo
- Performing simple calculations using different LEFT hand gestures through web cam.
![Alt Text](https://github.com/whatifif/handgesture/blob/master/draft-j/resources/demo.gif)

- Using Right hand to control the mouse cursor.
![Alt Text](https://github.com/whatifif/handgesture/blob/master/draft-j/resources/out-mouse.gif)

## Future Work
- Improve our Hand Detection, this can be extended to ultilise a Deep Learning Model, and get a more accurate feedback

- By using Haar cascade, the face can be detected and removed or only hands can be detected. Then the detection region for hands is not needed and we can move our body freely.

- Add reference points to catch a skin color and set it as a new skin color to detect. And while preprocessing, change the new skin color to the skin color used in training. In this way, the new skin color can be tracked correctly also.  

- Add 'unknown' class if the probability is under criteria. When classified as 'unknown', immediately capture next frame without waiting the next 10 frames. 

- Add more gestures such as raising 1st finger, index finger, index and middle finger, 1st and thumb funger 

- Need more data in training for various situations of the hand. Such as, different skin color, hand size, brightness, and oculus issues. This might modify the model struture if needed

- Advanced training method so as not to require too many data sets, such as using 3D hand model instead of 2D hand images for training.

- Establishing and propagating the standard Hand Gestures for mobile and remotely-controlled devices

## P.S. What will be the future of human in AI (Artificial Intelligence) age?
What will be the future of us, human in AI age? There will be no work which human have to do for living. We may have Universal Basic Income and have freedom to do what we like to do. AI may make an utopian world for human. Then to reach the utopian world as soon as possible, why not cooperate in developing AI rather than compete for limited resources and be greedy?  By using technology including AI, we can make our resources rich enough to be used by all human. Human will be multiplanetary species in future and there are infinite resources out there in universe. Lets make AI work for us, human and lets enjoy our lives as a human being.

