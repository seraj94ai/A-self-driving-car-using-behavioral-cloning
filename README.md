# Self-driving
## youtube tutorial
[![A self-driving car using behavioral cloning](https://github.com/seraj94ai/Self-driving/blob/master/scene00061.png)](https://youtu.be/T-gVwg90spc)


Project Description
In this project, I use a neural network to clone car driving behavior. It is a supervised regression problem between the car steering angles and the road images in front of a car.

Those images were taken from three different camera angles (from the center, the left and the right of the car).

The network is based on The NVIDIA model, which has been proven to work in this problem domain.

As image processing is involved, the model is using convolutional layers for automated feature engineering.


| Left-IMG | Centerleft-IMG | Right-IMG |
| :---         |     :---:      |          ---: |
| ![alt text](https://github.com/seraj94ai/Self-driving/blob/master/IMG/center_2019_02_23_20_23_56_553.jpg)   | ![alt text](https://github.com/seraj94ai/Self-driving/blob/master/IMG/Center_2019_02_23_20_23_56_553.jpg)     | ![alt text](https://github.com/seraj94ai/Self-driving/blob/master/IMG/right_2019_02_23_20_23_56_553.jpg)    |
  

| ###Layer (type)          | ###Output Shape           | ###Param # |
| :---                     |     :---:                 |    ---: |
| conv2d_6 (Conv2D)        | (None, 31, 98, 24)        | 1824    |
| conv2d_7 (Conv2D)        | (None, 14, 47, 36)        |21636    |
| conv2d_8 (Conv2D)        | (None, 5, 22, 48)         |43248    |
| conv2d_9 (Conv2D)        | (None, 3, 20, 64)         |27712    |
| conv2d_10 (Conv2D)       | (None, 1, 18, 64)         |36928    |
| flatten_2 (Flatten)      | (None, 1152)              |0        |
| dense_5 (Dense)          | (None, 100)               |115300   |
| dense_6 (Dense)          | (None, 50)                |5050     |
| dense_7 (Dense)          | (None, 10)                |510      |
| dense_8 (Dense)          | (None, 1)                 |11       |
|                          | Total params: 252,219     |      |


