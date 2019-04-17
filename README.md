# Group 10 Final Project - NAVARCH 568 W19
###### Xiaotong Chen, Deyang Dai, Yizhou Lu, and Joseph Yates
This project is created by Team 10, as its the final project for University of Michigan's NAVARCH 568, Winter 2019. The aim of this work is to replicate the IMU preintegration factor work completed in [Forster, Carlone, Dellaert, and Scaramuzza (2016)](https://ieeexplore.ieee.org/document/7557075). We then seek to validate this against the paper's implementation in the [Georgia Tech Smoothing and Mapping (GTSAM) library](https://bitbucket.org/gtborg/gtsam/overview). Additionally, we seek to test the IMU preintegration factor methodology on two relatively new datasets: IMU data from the UMich Biped Robotics Lab's [Cassie Blue](https://www.biped.solutions/research) robot, and the [KAIST Urban Dataset](http://irap.kaist.ac.kr/dataset/). With the KAIST dataset implementation, we also demonstrate the improvement that IMU preintegration offers over a baseline [ORB-SLAM2](https://arxiv.org/abs/1610.06475) implementation.

## Dependencies
This repo relies on two MATLAB toolboxes: MATLAB's own [Robotics System Toolbox](https://www.mathworks.com/products/robotics.html) and the [GTSAM Toolbox 3.2.0](https://borg.cc.gatech.edu/download.html#download). The latter is the MATLAB wrapper form of the [GTSAM library](https://bitbucket.org/gtborg/gtsam/overview). We include the GTSAM github repo as a submodule in our repo here; it may be compiled into the toolbox using [CMake](https://cmake.org/) (with [Boost](https://www.boost.org/) as a dependency to that compilation).
