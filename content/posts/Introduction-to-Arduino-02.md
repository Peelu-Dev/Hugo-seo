---
categories: ["Arduino"]
description: Arduino Tutorial for beginners to build the innovative products and use it in our daily life
author:
  name : "Peelu"
date: "2022-04-16"
linktitle: "Introduction to arduino-02"
type: 
  - post
  - posts
title : "Introduction to arduino-02"
featured_image: https://images.unsplash.com/photo-1553406830-ef2513450d76?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1031&q=80
tags: ['arduino','innovation']
weight : 10
series:  
  - Hugo 101
---

## Introduction

- ### Before we start our Tutorial my humble request is to use simulation softwares like Tinker Cad, Wokwi and Proteus as much as possible at the time of learning because nowadays we all are facing climate change, global-warming etc and we need to use less hardwares atleast at the time of learning or building the prototypes.

- ###  We will start our todays lesson with some basics and slowly move into advance today we are going to blink external LED with our Arduino board and enjoy the process of learning in a fun and exciting manner.

- ### To follow this lesson please follow  my previous lesson to understand well about Arduino Uno and its digital and analog pins so that we can use correctly and Breadboard and other parts of the hardware .

- ### Link to my previous course is given below or if you have that basic knowledge then follow this tutorial directly :-

[Introduction to Arduino-01](https://palashraghuwanshi.com/2022/introduction-to-arduino-01/)

- ## Why all we need to learn Arduino?

- ### Answer is pretty simple it actually solves multiple problems in any field whether its household, industrial, Natural, Medical and the list never finish and its quite interesting to make something amazing out of our imagination.

- ### Some of the examples are automated fish feeder, automated plant water system , smart things such as Home Automation, smart mirror and much more, whatever you think you can make out of it.

- ### Innovation takes time , because we all have to acquire the knowledge of that particular subject so that we can constantly experiments with the things we learn and nowadays softwares like Tinker Cad and wokwi simulators can easily reduce the cost of initial prototyping without purchasing hardwares to simulate what we learn.

- ### To be honest my everyday whenever I am learning Arduino or Experimenting is a Fun and Interesting day as I love to have that feeling of controlling things of my own.

- ### If I say Led to On for 1 second and Off for 300 micro seconds it will act according to it isn't it amazing we can do much more if we have the knowledge about it.

## Hardwares required  for this Project are given below:-

- ### Arduino Uno (which controls all the things according to our program or intructions )

- ### 1 LED (any colour of your choice you want)

- ### 1 resistor (220 ohm to limit the amount of current so that our LED will not damage)

- ### Solderless BreadBoard (to connect all the Hardware components)

- ### USB Cable (to program the Arduino Uno board)

- ### Some Jumper wires (to attach the pins)

## How to use Breadboard

![BreadBorad](https://cdn.pixabay.com/photo/2020/05/23/17/27/breadboard-5210635_960_720.jpg)

- ### All the (+) sign on a horizontal columns on the BreadBoard is connected with each other and can be used to give power supply to our arduino board.

- ### All the (-) sign on a horizontal columns on the BreadBoard is connected with each other and can be used to connect our Ground pin of our arduino board.

- ### All the 10 pins on middle of the BreadBoard divided in two parts in vertical rows are connected to each other to connect our different parts of our circuit to attach to it and make them work properly.

- ### If you wanted to know more about BreadBoard then follow this wonderful article written by science buddies link is given below:-

    [How to use a BreadBoard](https://www.sciencebuddies.org/science-fair-projects/references/how-to-use-a-breadboard)

## Circuit Diagram 

- ### Arduino Board(Gnd) -> BreadBoard(-)

- ### LED (Cathode leg) -> BreadBoard(-)

- ### LED (anode leg with 220 ohm resistor) -> Arduino Board digital pin (12) or any pin of your choice

- ### If you find any difficulty then follow my circuit given below:-

![Circuit Diagram](/1_LED_with_1_Resistor.png)

## External LED Blink Example

- ### First connect your ground pin to your (-) sign of the BreadBoard then connect your USB cable to the computer to upload the sketch.

- ### Then connect your led (cathode leg) to (-) sign of the BreadBoard with jumper wire.

- ### Then connect your led (annode leg with 220 ohm resistor) with jumper wire to digital Pin number 12 of your Arduino Board and then upload the code given below to see how Led is turning On and Off according to our instruction.

- [External LED Blink](https://github.com/Peelu-Dev/Begiiners-guide-to-arduino/blob/main/1_LED_with_1_Resistor/1_LED_with_1_Resistor.ino)

## Code Explanation

- ### First I have made variable name ledWithResistor and store its value in pin number 12.

- ### Then there are two function which is void setup and void loop. void setup is mainly used to write code that will run only once and void loop is main used to write code that will run always untill we break the code or disconnect the board.

- ### Then I have set our ledWithResistor variable to OUTPUT with the help of pinMode and pinMode is generally used for either OUTPUT or INPUT.

- ### Then I have turn ON the external led with digitalWrite function and set its value to HIGH and then wait for two second with delay function and then I have turn OFF the external led with digitalWrite function and set it to LOW and then wait for 1 second and that's the whole process of external led Blinking effect.

## Tinker CAD Simulation

- ### Sign up for an free account on Tinker CAD website [TinkerCad](https://www.tinkercad.com/join) and then tap on circuits below and then tap on create new circuit.

- ### If you have any difficulty in circuit diagram then follow my circuit diagram given below:-

![Circuit Diagram](/1_LED_with_1_Resistor.png)

- ### Then search for Arduino Uno in search box and drag it to blank space and then drag BreadBoard and led and 220 ohm resistor and then tap on code and select only text code editor and paste my code link is given below in code editor.

- [external led Blink](https://github.com/Peelu-Dev/Begiiners-guide-to-arduino/blob/main/1_LED_with_1_Resistor/1_LED_with_1_Resistor.ino)

- ### Then click on start simulation and you will see the external LED on the BreadBoard is blinking according to your code and don't forget to change the delay code to see the difference each time and start enjoying the process.




