---
categories: ["Arduino"]
description: Arduino Tutorial for beginners to build the innovative products and use it in our daily life
author:
  name : "Peelu"
date: "2022-04-13"
linktitle: "Beginner Guide to Arduino-01"
type: 
  - post
  - posts
title : "Beginner Guide to Arduino-01"
tags: ['arduino','innovation']
weight : 10
series:  
  - Hugo 101
---

## Introduction

![Arduino](https://images.unsplash.com/photo-1553406830-ef2513450d76?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1031&q=80)

- ### Arduino is an open source hardware and software company which is mainly used for creating different types of interesting projects and learn more about how both hardware and software works to make amazing products for the needy ones.Arduino boards are able to read inputs - light on a sensor, a finger on a button, or a Twitter message - and turn it into an output - activating a motor, turning on an LED, publishing something online. You can tell your board what to do by sending a set of instructions to the microcontroller on the board. To do so you use the Arduino programming language (based on Wiring), and the Arduino Software (IDE), based on Processing.

- ### Over the years Arduino has been the brain of thousands of projects, from everyday objects to complex scientific instruments. A worldwide community of makers - students, hobbyists, artists, programmers, and professionals - has gathered around this open-source platform, their contributions have added up to an incredible amount of accessible knowledge that can be of great help to novices and experts alike.

## Why Arduino?

- ### Inexpensive - Arduino boards are relatively inexpensive compared to other microcontroller platforms.As they are made for fast prototyping they are easily available at anywhere in the world at cheap price even duplicates are also very good to use for learning and they are available at minimum prices.

- ### Cross-platform - The Arduino Software (IDE) runs on Windows, Macintosh OSX, and Linux operating systems. Most microcontroller systems are limited to Windows.

- ### Clear programming environment - The Arduino Software (IDE) is easy-to-use for beginners, yet flexible enough for advanced users to take advantage of as well. For teachers, it's conveniently based on the Processing programming environment, so students learning to program in that environment will be familiar with how the Arduino IDE works.

## Boards

### There are different kinds of Arduino Boards available in the market but we will use Arduino Uno through Out this course i will explain about this board:-

## Arduino Uno

- ### Arduino/Genuino Uno is a microcontroller board based on the ATmega328P IC. It has 14 digital input/output pins (out of which 6 can be used as PWM outputs), 6 analog inputs, a 16 MHz quartz crystal, a USB connection, a power jack, an ICSP header and a reset button.

- ### It contains everything needed to support the microcontroller; simply connect it to a computer with a USB cable or power it with a AC-to-DC adapter or battery to get started.

- ### You can tinker with your UNO without worring too much about doing something wrong, worst case scenario you can replace the chip for a few dollars and start over again.

- ### "Uno" means one in Italian and was chosen to mark the release of Arduino Software (IDE) 1.0. The Uno board and version 1.0 of Arduino Software (IDE) were the reference versions of Arduino, now evolved to newer releases. 

- ### The Uno board is the first in a series of USB Arduino boards, and the reference model for the Arduino platform; for an extensive list of current, past or outdated boards see the Arduino index of boards.

## Arduino IDE

- ### Download the Arduino IDE from Arduino official website link is given below :-

[Arduino IDE ](https://www.arduino.cc/en/software)

- ### The editor contains the four main areas:

- #### 1. A Toolbar with buttons for common functions and a series of menus. The toolbar buttons allow you to verify and upload programs, create, open, and save sketches, and open the serial monitor.

- #### 2. The message area, gives feedback while saving and exporting and also displays errors.

- #### 3. The text editor for writing your code.

- #### 4. The text console displays text output by the Arduino Software (IDE), including complete error messages and other information.

- ### The bottom right-hand corner of the window displays the configured board and serial port.

![image showing arduino interface](https://docs.arduino.cc/static/ebf961f81c305e826d52e3401863b48e/4ef49/arduino-ide-interface.png)

- ### Now that you are all set up, let’s try to make your board blink!

- #### 5. Connect your Arduino or Genuino board to your computer.

- #### 6. Now, you need to select the right core & board. This is done by navigating to Tools > Board > Arduino AVR Boards > Board. Make sure you select the board that you are using. If you cannot find your board, you can add it from Tools > Board > Boards Manager.


![how to connect to board](https://docs.arduino.cc/static/72ed26100bd60c7c0bb07779d3c6a96d/4ef49/install_avr_02.png)

- ### 7. Now, let's make sure that your board is found by the computer, by selecting the port. This is simply done by navigating to Tools > Port, where you select your board from the list.

![Selecting a port](https://docs.arduino.cc/static/6f0ce64a330509eeeebaaa899b81405a/4ef49/install_avr_03.png)

### If you want more details then visit the official website :-

[Arduino](https://docs.arduino.cc/learn/starting-guide/the-arduino-software-ide#using-the-offline-ide-1xx)

## OnBoard LED Blink example

- ### Connect your Arduino Uno Board with pin number 13 and then connect your USB cable to the computer to upload the sketch.

- ### Copy the code from my repository [Onboard LED Blink](https://github.com/Peelu-Dev/Begiiners-guide-to-arduino/tree/main/onBoardLed_blink) and upload to your arduino IDE.

- ### When your code has been compiled successfully then you will see the onBoard LED on the Arduino board will ON for half second and Off for 1 second.

- ### Change the delay to see the difference of how the led is blinking according to your intention. Note that delay will take the time in milliseconds so 1000 milliseconds is 1 second and 500 milliseconds is half second.

## Code Explanation

- ### First I have made a variable name onBoardLed and store the pin number 13 in it.

- ### Then there are two function which is void setup and void loop. void setup is mainly used to write code that will run only once and void loop is main used to write code that will run always untill we break the code or disconnect the board.

- ### Then I have set our onBoardLED to OUTPUT with the help of pinMode and pinMode is generally used for either OUTPUT or INPUT.

- ### Then I have ON the onBoardLED with digitalWrite function and set it to HIGH and then wait for half second with delay function and then I have OFF the onBoardLED with digitalWrite function and set it to LOW and then wait for 1 second and that's the whole process of Blinking effect.


## Tinker CAD Simulation

- ### Sign up for an free account on Tinker CAD website [TinkerCad](https://www.tinkercad.com/join) and then tap on circuits below and then tap on create new circuit.

- ### Then search for Arduino Uno in search box and drag it to blank space and then tap on code and select only text code editor and paste my code [my code](https://github.com/Peelu-Dev/Begiiners-guide-to-arduino/tree/main/onBoardLed_blink) in code editor.

- ### Then click on start simulation and you will see the onboard LED written L on the Arduino is blinking according to your code and don't forget to change the delay code to see the difference.



