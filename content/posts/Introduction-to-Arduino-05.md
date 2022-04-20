---
categories: ["Arduino"]
description: Arduino Tutorial for beginners to build the innovative products for the needy ones and use it in our daily life
author:
  name : "Peelu"
date: "2022-04-20"
linktitle: "Introduction to Arduino-05"
type: 
  - post
  - posts
title : "Introduction to Arduino-05"
tags: ['arduino','innovation']
featured_image: https://images.unsplash.com/photo-1485827404703-89b55fcc595e?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80
weight : 10
series:  
  - Hugo 101
---

## Introduction

- ### Before we start our Tutorial my humble request is to use simulation softwares like Tinker Cad, Wokwi and Proteus as much as possible at the time of learning because nowadays we all are facing climate change, global-warming etc and we need to use less hardwares atleast at the time of learning or building the prototypes.

- ### So in this lesson we will discuss about different types of Data Types and its working in deep so that we can use effectively in developing high quality innovative products for the needy ones.

- ### Data types are quite useful in many scenarios of our real world situations like controlling servo motors to rotate at the certain degree of angles and we can easily store servo motor position inside those different datatypes.

## Different Data Types in Arduino and their workings

- ### Int :- Integer is a popular and most used data type in any programming language and you can understand pretty well if you are learning arduino because you are dealing with hardware and software directly.

    - ### Lets imagine if you want to control five different leds and their states or working principle are basically either ON and OFF and their range is quite low so we can easily store those Leds inside int data type easily.

    - ### First we will store these five pins inside int data type and then make it blink.

    ![Light Bulbs](https://images.unsplash.com/photo-1547393947-a6a221f74e59?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80)

    - ### int led1 = 13;
    - ### int led1 = 12;
    - ### int led1 = 11;
    - ### int led1 = 10;
    - ### int led1 = 9;

    - ### void setup()

    - ### {

    - ###  pinMode(led1,OUTPUT);
    - ###  pinMode(led2,OUTPUT);
    - ###  pinMode(led3,OUTPUT);
    - ###  pinMode(led4,OUTPUT);
    - ###  pinMode(led5,OUTPUT);

    - ### }

    - ### void loop()

    - ### {
    - ### // First we will ON the five Leds
    - ### digitalWrite(led1,HIGH); 
    - ### digitalWrite(led2,HIGH); 
    - ### digitalWrite(led3,HIGH); 
    - ### digitalWrite(led4,HIGH); 
    - ### digitalWrite(led5,HIGH); 
    - ### // In Arduino delay uses milli seconds so we need to give 1000 milli seconds so that it will wait for 1 second
    - ### delay(1000);    
    - ### // Then we will OFF the five Leds        
    - ### digitalWrite(led1,LOW);  
    - ### digitalWrite(led2,LOW);
    - ### digitalWrite(led3,LOW);
    - ### digitalWrite(led4,LOW);
    - ### digitalWrite(led5,LOW);    
    - ### delay(1000);
    - ### With this code we can blink five leds together with the help of int data type
    - ### }

- ### float :- float data type can be very useful in reading various types of sensor and storing inside float and they can very easily store those floating point values inside them.

    - ### lets understand with real life example if we want to store the readings of dht11 or dht22 temperature sensor then we get floating point decimal number with temperature sensor readings.

    - ### Now we will see how to program dht11 temperature sensor and see the readings in serial monitor, you can easily program in any simulation softwares like Tinker Cad, Wokwi or Proteus.

    ![Tempearure](https://images.unsplash.com/photo-1622069873046-39550b57c903?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80)

    - ### #include<DHT.h>
    - ### #define DHTPIN 2 
    - ### #define DHTTYPE DHT11
    - ### // initialise the sensor
    - ### DHT dht(DHTPIN, DHTTYPE);

    - ### void setup()

    - ### {


    - ### // Establishing Serail communication so that we can see the result in our serial monitor
    - ### Serial.begin(9600);
    - ### Serial.println("Testing DHT11 temperature sensor");
    - ### dht.begin();

    - ### }

    - ### void loop()

    - ### {
    
    - ###   // Wait a few seconds between measurements.
    - ### delay(2000);
    - ### // reading dht11 temperature sensor data with float data type
    - ### // reading humidity from sensor
    - ### float h = dht.readHumidity();
    - ### //reading temperature in  celcius from sensor
    - ### float t = dht.readTemperature();
    - ### //reading temperature in Fahrenheit from sensor
    - ### float f = dht.readTemperature(true);
    - ### // Check if any reads failed and exit early (to try again).
    - ###  if (isnan(h) || isnan(t) || isnan(f))
    - ### {

    - ### Serial.println(F("Failed to read from DHT sensor!"));
    - ### return;    

    - ### }

    - ### // Compute heat index in Fahrenheit (the default)
    - ### float heat_index_in_fahrenheit = dht.computeHeatIndex(f, h);
    - ### // Compute heat index in Celsius (isFahreheit = false)
    - ### float heat_index_in_celcius = dht.computeHeatIndex(t, h, false);
    
    - ### Serial.print(F(" Humidity: "));
    - ### Serial.print(h);
    - ### Serial.print(F("%  Temperature: "));
    - ### Serial.print(t);
    - ### Serial.print(F("C "));
    - ### Serial.print(f);
    - ### Serial.print(F("F  Heat index: "));
    - ### Serial.print(hic);
    - ### Serial.print(F("C "));
    - ### Serial.print(hif);
    - ### Serial.println(F("F"));

    - ### // With this code you can easily store the tempeature reading from dht11 sensor and see it in a Serial monitor in Arduino IDE, Tinker Cad, Wokwi simulator or in Proteus
    - ### }

- ### long:- Long data type is also quite useful when it comes to read large amount of numbers and it is the extended version of float data type which is more powerful than float.

    - ### let me walk you through an example where we will read the value of Ultrasonic HCSR-04 distance sensor which is capable of transmit the distance infront of him and gives relevant information with their readings.

    - ### Now we will see how to program HCSR-04 distance sensor and see the readings in serial monitor, you can easily program in any simulation softwares like Tinker Cad, Wokwi or Proteus without having hardware.

    ![Robotics car with distance sensor](https://images.unsplash.com/photo-1561144257-e32e8efc6c4f?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80)

    - ### // setting trigger and echo pin with const and int data type beacuse we are not going to change these pins
    - ### const int triggerPin = 9;
    - ### const int echoPin = 10;
    - ### // reading duration of the sensor with long data type
    - ### long duration;
    - ### int distance;

    - ### void setup() 

    - ### {

    - ### // put your setup code here, to run once:
    - ### pinMode(triggerPin,OUTPUT);
    - ### pinMode(echoPin,INPUT);
    - ### // Establishing Serail communication so that we can see the result in our serial monitor
    - ### Serial.begin(9600);

    - ### }

    - ### void loop() 
    
    - ### {

    - ### // put your main code here, to run repeatedly:

    - ### // clearing the trigger pin if it is already active
    - ### digitalWrite(triggerPin,LOW);
    - ### // giving very small amount of delay in micro seconds
    - ### delayMicroseconds(2); 

    - ### digitalWrite(triggerPin,HIGH);
    - ### delayMicroseconds(10);
    - ### digitalWrite(triggerPin,LOW);
    - ### // reading duration with pulseIn builtin function
    - ### duration = pulseIn(echoPin,HIGH);
    - ### Finding exact distance with this formula
    - ### distance = duration * 0.034/2 ;
    - ### // Printing distance on serail monitor
    - ### Serial.print("Distance : ");
    - ### Serial.println(distance);
  
    - ### }

### We will discuss more data types with some of the real life examples in next Blog as this blog will become quite lengthy. If you have any question then comment it down in comment box or dm me on my social media channels icons with links are given on my home page.

[HomePage](https://palashraghuwanshi.com/)



