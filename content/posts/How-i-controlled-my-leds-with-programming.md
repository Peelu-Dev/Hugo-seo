---
categories: ["Arduino"]
description: How i learned to write my first magical code that is controlling LEDs according to my thinking.
author:
  name : "Peelu"
date: "2022-04-07"
linktitle: "How i Controlled my LEDs with low or no programming knowledge and it really excites me"
type: 
  - post
  - posts
title : "How i Controlled my LEDs with low or no programming knowledge and it really excites me"
weight : 10
series:  
  - Hugo 101
---

## Introduction

![Arduino](https://images.unsplash.com/photo-1553406830-ef2513450d76?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1031&q=80)

- When we all talk about intelligence, we can't forget the Humans and their Brains as we have developed the things whenever we have find those little problems associated with it and will find the solution according to it.

- Once upon a time a tinkerer or thinker find a problem and his or her problem starts with why the LEDs or lights have only the two states On and OFF and is there any way to control the LEDs or Lights according to our needs and wants.

- Then he or she has done some research on the internet and in initial days he or she doesn't found much on the internet but their hard work and effort went successful when they understand that we Humans have to give our brains to LEDs and then control according to it.

- Then they have done some research on the internet and find that computers understand some programming languages that they need to learn and have to acquire some knowledge of electronics and  micro-controllers which can control the LEDs according to our commands and wants.

## Hardwares required for this project are given below :- 

![Innovation starts from here](https://images.unsplash.com/photo-1603732551658-5fabbafa84eb?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80)

### Arduino Uno or any micro-controller

### Some LEDs

### 220 Ohms resitors

### Breadboard

### USB Cable to program the arduino

### some jumper wires to connect the LEDs, resistors and jumper wires.

## Softwares required for this project are given below :-

### Arduino IDE with hardware


- Arduino IDE to hands on learning with physical hardwares to feel the magic infront of our eyes otherwise online simulation is enough to do this project easily.

### TinkerCad for online simulation without hardware

- In TinkerCad we do not need or required any hardware as all hardware and code editor is provided by the TinkerCad itself for simulating our projects without worry about HardWares to purchase.

### BreadBoard

- If you want to learn more about BreadBoard and its functionality just read the wonderful article written by sparksfun link is given below :-
[How to Use a Breadboard](https://learn.sparkfun.com/tutorials/how-to-use-a-breadboard/all)

### Circuit Diagram

![Circuit Diagram](/arduino.png)

- First, connect the jumper wire to ground pin or gnd pin of the arduino and ground signal on the breadboard(-) which will connect all the ground pins together and make sure to unplug the board when making the circuit diagram.

- Then place the led on middle of the breadboard and connect the cathode(small leg of the led) to the ground pin which is minus (-) sign on the breadboard easily.

- Then connect the annode(long leg of the led) with 220 ohm resistor attached to it pin number 12 or any pin of the arduino to program it according to our needs and wants.

- Follow my circuit diagram if you have any problems associated with it or if you stuck anywhere while making circuit diagram:-

![Controlling LED](/arduino.png)

### Arduino IDE

- Download the arduino IDE from its official website [Arduino IDE](https://www.arduino.cc/en/software) and after downloading open the code editor and follow the steps to control LED according to how you wanted to control.

- When you open Arduino Code editor for the first time you will see the interface with code written like this :-

- void setup(){
  // put your setup code here, to run once:
}

- void loop(){
  // put your loop code here, to run repeatedly:
}

- This code simply means if you want to write the code which will run only once like setup the LED pin to pin number 12 so you have to write in this void setup block and if you want to run the code multiple times like blinking the LED again and again then write the code in void loop block.

- When you see those two forward slashes like this // are comments which simply means that computer will ignore these lines at the run time and they are usually written to understand our own code well.

## Magical Code to control a single LED 

- // Arduino code

- int ledWithResistor = 12;

- void setup()
  {

    pinMode(ledWithResistor, OUTPUT);
    
  }

- void loop()
  {

    digitalWrite(ledWithResistor, HIGH); // on the led

    delay(2000); // Wait for 2000 millisecond(s)

    digitalWrite(ledWithResistor, LOW);

    delay(1000); // Wait for 1000 millisecond(s)
    
  }

  ## Let me explain this magical code

  - First i have declared my led pin with resistor connected to it in a variable called ledWithResistor which will store the value of a pin number.

  - Then in void setup function i have written my pinMode with our variable and set it to OUTPUT mode so that our computer will recognize that we need to glow the LED.

  - Then in void loop function i have written  digitalWrite(ledWithResistor, HIGH); which simply means On the LED and delay(2000); wait for 2 seconds and digitalWrite(ledWithResistor, LOW); off the led and delay(1000); and wait for 1 second to have a blinky effect as we have written this code in void loop function it will run the code in loop and will not stop until we disconnect the arduino.

  - You can always change the code and see how the things are working like change the  delay to 250 and see how fast it is working and most imprtant part is to have a fun whenever you are tinkering with arduino.


  ## TinkerCad Code

- int ledWithResistor = 12;

- void setup()
  {

    pinMode(ledWithResistor, OUTPUT);
    
  }

- void loop()
  {

    digitalWrite(ledWithResistor, HIGH); // on the led

    delay(2000); // Wait for 2000 millisecond(s)

    digitalWrite(ledWithResistor, LOW);

    delay(1000); // Wait for 1000 millisecond(s)
    
  }

- Open your TinkerCad account make the circuit and write this code in code section and click on start simulation button to see the Blinky effect in simulation without hardware.





