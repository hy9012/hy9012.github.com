---
title:  "우분투에서 그래픽카드 설치하기"
date:   2015-04-15 09:16:00
categories: example
---

**NVIDIA X Server Settings 설치**

    * 우분투 소프트웨어 센터에서 NVIDIA X Server Sttings 검색해서 설치

**NVIDIA 그래픽카드 드라이버 설치**
    * 1. sudo add-apt-repository ppa:xorg-edgers/ppa
    * 2. sudo apt-get update
    * 3. sudo apt-get install nvidia-349 (CUDA설치를 위해서는 346이상 설치)
    * 4. 재부팅
