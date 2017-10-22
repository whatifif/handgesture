# Use hand gestures to controll keyboard/mouse


## Project Outline

- Using hand gestures to controll keyboard cam

![](http://4.bp.blogspot.com/-cnzK8dupTCs/UXP7ApP-ppI/AAAAAAAADtA/9rYB_qv04wI/s1600/control+your+PC+through+Webcam+ztuts.com.png)

- Using hand movements and gesture to control mouse/clicks though cam

![](https://thetechhacker.com/wp-content/uploads/2013/08/Control-Your-Home-With-Gesture-And-Voice-Using-Flowton.jpg)



## Technical Details

### Main Dependencies:
 - Python 2.7
 - Opencv 3.2.0
 - MxNet 0.11.0
 - Numpy 1.13.1
 - Pandas 0.20.3
 -  ..

### Difficulties
 - Very few existing dataset fits our purpose. Therefore, we have to capture the hand picture, and do the labeling. A.k.a, we will have to make the dataset our own

 - Tracking and recognizing hand are 2 challenges in this project, and each requires large amount of time to work on. Therefore, in this project, we are firstly focusing on Recognition, and used a just feasible approach for Hand Detection for saving time. 

 - Model selections, especially on building a Neural Nework architecture. That is, if the Neural Network is too "deep", it takes long time to converge, and also is not suitable in real-time cameras. While single-layer NN does not performing good enough
 

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


## Our Progress

- Use Left hand for keyboard, Right hand for mouse

- At current stage, Left hand can be used for around 30 different keys in the keyboard, based on the hand gesture, and their angles in the picture




## Demo
- Performing simple calculations using different LEFT hand gestures through web cam.
![Alt Text](https://github.com/whatifif/handgesture/blob/master/draft-j/resources/demo.gif)

- Using Right hand to control the mouse cursor.
![Alt Text](https://github.com/whatifif/handgesture/blob/master/draft-j/resources/out-mouse.gif)

## Future Work
- Improve our Hand Detection technical, this can be extended to ultilise a Deep Learning Model, and get a more accurate feedback

- Determine the classes (keys) in a more effecient/effective way

- Need more data in training for various situations of the hand. Such as, different skin color, hand size, brightness, and oculus issues. This might modify the model struture if needed














