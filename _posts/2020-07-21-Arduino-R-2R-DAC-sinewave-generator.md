---
title: 2-2R DAC sinewave generator with Arduino
author: Karol
layout: post
hide: true
---

<div style="text-align: justify"> R - 2R is one of the simpliest way to perform digital to analog conversion. In combination with Arduino,
which lacks a build-in DAC, it seems to be a good thing. Let's make a simple example with this type of DAC creating sinewave generator and using Citron Maker UNO.   </div> 

<div style="text-align: justify">
Firstly, I made a circuit on breadboard, checked if everything is working and so on, but now I will show and discuss the schematic
</div>

<img src="{{'assets/images/r-2r sine generator.jpg' | relative_url}}" alt="schematic">

<div style="text-align: justify">
The resistors R1-R16 form the discussed digital to analog converter. <a href="https://www.youtube.com/watch?v=Pc1aFloxSMw">Here</a> is good wxplained how R-2R DAC works.
I buid 8-bit DAC, so maximum voltage value (5V) is represented as 255. The resolution achieved by 8-bit DAC is 5V/2<sup>8</sup> and this equals 0.0195 Volts. It's quite good. The resultion can be easily increased by adding more resistors in ladder, but we are limited by arduino output pins. The output resistance of DAC equals 1k&Omega. R25 controls the output amplitude
</div>

