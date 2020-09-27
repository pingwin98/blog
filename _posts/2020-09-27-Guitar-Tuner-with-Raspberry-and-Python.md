---
title: Guitar Tuner With Raspberry and Python
author: Karol
layout: post
icon: fa-code
tags: Raspberry Pi, Python, DIY, Guitar
hide: false
---

<div style="text-align: justify">
As one of projects on the university I've made my own guitar tuner using Raspberry Pi. Everything was coded in Python 3. The tuner is packed up in 3d printed enclosure (but it's only a prototype, needs to be polished :) ). 

<p align="center">
<img src="{{'assets/images/guitar_tuner/ready_tuner.jpg' | relative_url}}" alt="guitar tuner using RPI" width="100%" height="auto">
</p>

<h1>Things I used to build guitar tuner</h1>
<ul>
<li>Raspberry Pi 3B+,</li>
<li>USB sound card,</li>
<li>Tie clip microphone,</li>
<li>LED diode,</li>
<li>2x buttons, </li>
<li>2x16 LCD display,</li>
<li>10k potentiometer </li>
</ul>

USB external soundcard is needed as Rpi doesn't have microphone input. As microphone I used tie clip mic - it can be attachet easily to guitar near the strings. LED diode is for indication. Button is needed for turning on and off the tuner. Potentiometer is needed for LCD display.

<p align="center">
  <a href="http://www.youtube.com/watch?v=jrpyii77ICg&t=4s">Video with the tuner.</a>
</p>

In the video above it is visible how the tuner works. After startup you can turn on tuner with the button. The second button is used to turn off the tuner when it is running, or shutdown the Linux system when the Rpi is waiting for turning on  the tuner.

The program responsible for tuning is written in python. The audio is collected using pyaudio lib. Then audio signal is filtrated and transformed with Fourier Transformation. With finding the peaks in Fourier transform of a signal, the program matches string frequency with musical notes. 

In the midlle of the screen current note, and arrow(tune up, or down) is displayed. On the left we have string frequency and on the right there is an octave of the played note. 

The tuners accuarcy is about +/-0.3 Hz. But the accuarcy can be easily increased with zero-padding in Fourier Transformation. Anyway 0.3Hz is quite good and makes the tuner very fast (I didn't try increasing accuarcy more than 0.3 Hz but i thing it won't strongly affect the speed of tuner).

Some more photos below:

<p align="center">
<img src="{{'assets/images/guitar_tuner/ready_tuner2.jpg' | relative_url}}" alt="guitar tuner using RPI 2 " width="100%" height="auto">
</p>

<p align="center">
<img src="{{'assets/images/guitar_tuner/tuner_down.jpg' | relative_url}}" alt="guitar tuner bottom side" width="100%" height="auto">
</p>

<p align="center">
<img src="{{'assets/images/guitar_tuner/tuner_inside.jpg' | relative_url}}" alt="guitar tuner inside" width="100%" height="auto">
</p>

I will post the code if there will be request - email me with the form on the main page ;)

</div>
