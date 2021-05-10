---
title: BLDC motor test stand
author: Karol
layout: post
icon: fa-wrench
tags: Raspberry Pi, Python, Arduino, BLDC motor
hide: false
---

<div style="text-align: justify">
This project was made as part of my thesis at  college. The main objective of this project was to design and create test stand which was to be used to conduct research on BLDC motors. The basic assumption of the designed test stand was possibility of testing motors with a power of up to 2 kW used in model making and motors built into the wheel hub with a power of up to 400 W.

The test bench enables:
- Measurment of supply voltage;
- Measurment of supply current;
- Measurment of motor temperature;
- Measurment of motor torque;
- Measurment of motor rotational speed;
- Controlling motor's rotational speed;
- Creating motors output characteristics;

During the project process, the braking method of the tested engine, the mechanical construction of the stand, the measurement and control system were considered, and the required components were selected. For the braking of the tested motor, the use of a second brushless motor was planned. The designed structure includes three properly selected toothed belt drives. A universal stand of the tested engines was also designed, which were made by a professional manufacturer. Basic calculations were also carried out to check the strength of the designed contruction (mainly the shafts and belt drives). The measurement and control system was based on the Raspberry Pi and Arduino platforms. The project resulted in the creation of a working prototype of the test stand, together with the software written in Python language. The software has also been developed with a graphical interface using the tools provided by the PyQt5 library.

The project was sponsored by company which needed such a test stand for their research. The created prototype of test stand fully met its assumptions. 

<p align="center">
<img src="{{'assets/images/bldc_motor_test_stand/1.png' | relative_url}}" alt="test stand render" width="100%" height="auto">
</p>

<p align="center">
<img src="{{'assets/images/bldc_motor_test_stand/6.png' | relative_url}}" alt="test stand render #2" width="100%" height="auto">
</p>

Figures above show the 3D model of test stand made in Inventor Pro during designing process. There are photos of ready prototype:

<p align="center">
<img src="{{'assets/images/bldc_motor_test_stand/ready_1.jpg' | relative_url}}" alt="test stand #1" width="100%" height="auto">
</p>

<p align="center">
<img src="{{'assets/images/bldc_motor_test_stand/ready_2.jpg' | relative_url}}" alt="test stand #2" width="100%" height="auto">
</p>

<p align="center">
<img src="{{'assets/images/bldc_motor_test_stand/electronics.jpg' | relative_url}}" alt="test stand electronics" width="100%" height="auto">
</p>

Here is test stand with hub motor mounted:
<p align="center">
<img src="{{'assets/images/bldc_motor_test_stand/hub.jpg' | relative_url}}" alt="test stand during tests" width="100%" height="auto">
</p>

The gui:
<p align="center">
<img src="{{'assets/images/bldc_motor_test_stand/gui.png' | relative_url}}" alt="test stand gui" width="100%" height="auto">
</p>

</div>