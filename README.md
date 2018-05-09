# Face_Recognition
## ---------------차례-----------------
### 1. 라즈베리파이 파이썬환경설정
### 2. opencv 환경설정
### 3. pip3 환경설정
## ------------------------------------
***
## 1. 라즈베리 환경설정
### (1) ubuntu_mate update & upgrade (우분투 최신버전 유지)
    $ sudo apt-get install update
    $ sudo apt-get install upgrade
***    
### (2) install opencv dependencies (opencv 의존성 설치)
    $sudo apt-get purge  libopencv* python-opencv
    $sudo apt-get autoremove
    $sudo apt-get install build-essential cmake
    $sudo apt-get -y install pkg-config libjpeg-dev libtiff5-dev libjasper-dev libpng12-dev libavcodec-dev libavformat-dev libswscale-dev libxvidcore-dev libx264-dev libxine2-dev libv4l-dev v4l-utils libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev libqt4-dev libgtk2.0-dev libgtk-3-dev mesa-utils libgl1-mesa-dri libqt4-opengl-dev libatlas-base-dev gfortran libeigen3-dev python3-dev python3-numpy libatlas-base-dev gfortran
***
