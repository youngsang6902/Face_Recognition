# Face_Recognition
>## ---------------차례-----------------
>### 1. 라즈베리파이 파이썬환경설정
>### 2. opencv 환경설정
>### 3. pip3 환경설정
>## ------------------------------------
***
## 1. 라즈베리 환경설정
### Ubuntu_mate update & upgrade (우분투 최신버전 유지)
    $ sudo apt-get install update
    $ sudo apt-get install upgrade
***    
## 2. Opencv 환경설정
### Install opencv dependencies (Opencv 의존성 설치)
    $ sudo apt-get purge  libopencv* python-opencv
    $ sudo apt-get autoremove
    $ sudo apt-get install build-essential cmake
    $ sudo apt-get -y install pkg-config libjpeg-dev libtiff5-dev libjasper-dev libpng12-dev libavcodec-dev libavformat-dev libswscale-dev libxvidcore-dev libx264-dev libxine2-dev libv4l-dev v4l-utils libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev libqt4-dev libgtk2.0-dev libgtk-3-dev mesa-utils libgl1-mesa-dri libqt4-opengl-dev libatlas-base-dev gfortran libeigen3-dev python3-dev python3-numpy libatlas-base-dev gfortran
***
### Download the opencv source (Opencv 소스 다운로드)
    $ wget -O opencv.zip https://github.com/opencv/opencv/archive/3.1.0.zip
    $ unzip opencv.zip
    $ wget -O opencv_contrib.zip https://github.com/opencv/opencv_contrib/archive/3.1.0.zip
    $ unzip opencv_contrib.zip
***
### Compile in the opencv directory
    $ cd opencv-3.1.0/
    $ mkdir build
    $ cd build
    $ cmake -D CMAKE_BUILD_TYPE=RELEASE \ 
    -D CMAKE_INSTALL_PREFIX=/usr/local \
    -D WITH_TBB=OFF \
    -D WITH_IPP=OFF \
    -D WITH_1394=OFF \
    -D BUILD_WITH_DEBUG_INFO=OFF \
    -D BUILD_DOCS=OFF \
    -D INSTALL_C_EXAMPLES=ON \
    -D INSTALL_PYTHON_EXAMPLES=ON \
    -D BUILD_EXAMPLES=OFF \
    -D BUILD_TESTS=OFF \
    -D BUILD_PERF_TESTS=OFF \
    -D WITH_QT=ON \
    -D WITH_OPENGL=ON \
    -D OPENCV_EXTRA_MODULES_PATH=../../opencv_contrib-3.1.0/modules \
    -D WITH_V4L=ON  \
    -D WITH_FFMPEG=ON \
    -D WITH_XINE=ON \
    -D BUILD_NEW_PYTHON_SUPPORT=ON \
    ../
***

