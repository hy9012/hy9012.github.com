---
title:  "우분투에서 OpenCV 설치하기"
date:   2015-04-15 14:33:00
categories: ubuntu
---

#Ubuntu가 최신상태인지 확인

-----------

> $ sudo apt-get update && sudo apt-get upgrade && sudo apt-get dist-upgrade && sudo apt-get autoremove

</br>
#의존관계 설치하기

-----------

### Build tools

> $ sudo apt-get install build-essential cmake

### GUI

> $ sudo apt-get install qt5-default libvtk6-dev

### Media I/O

> $ sudo apt-get install zlib1g-dev libjpeg-dev libwebp-dev libpng-dev libtiff5-dev libjasper-dev libopenexr-dev libgdal-dev

### Video I/O

> $ sudo apt-get install libdc1394-22-dev libavcodec-dev libavformat-dev libswscale-dev libtheora-dev libvorbis-dev libxvidcore-dev libx264-dev yasm libfaac-dev libopencore-amrnb-dev libopencore-amrwb-dev libv4l-dev libxine-dev

### Algebra libraries

> $ sudo apt-get install libtbb-dev libeigen3-dev

### Python

> $ sudo apt-get install python-dev python-tk python-numpy python3-dev python3-tk python3-numpy

### Java

> $ sudo apt-get install ant default-jdk

</br>

#OpenCV 설치하기

------------


> $ git clone https://github.com/Itseez/opencv.git
>
> $ cd opencv
>
> $ mkdir release
>
> $ cd release
>
> $ cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local ..
>
> $ make (설치 실패시 sudo make해보기)
>
> $ sudo make install

</br>

#Trouble shooting

---------------

### Python에서 안될 때

> $ sudo apt-get install python-opencv

