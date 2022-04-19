---
categories: ["Arduino"]
description: Arduino Tutorial for beginners to build the innovative products for the needy ones and use it in our daily life
author:
  name : "Peelu"
date: "2022-04-19"
linktitle: "Introduction to Arduino-04"
type: 
  - post
  - posts
title : "Introduction to Arduino-04"
tags: ['arduino','innovation']
featured_image: https://images.unsplash.com/photo-1603732551658-5fabbafa84eb?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80
weight : 10
series:  
  - Hugo 101
---

## Introduction

- ### Before we start our Tutorial my humble request is to use simulation softwares like Tinker Cad, Wokwi and Proteus as much as possible at the time of learning because nowadays we all are facing climate change, global-warming etc and we need to use less hardwares atleast at the time of learning or building the prototypes.

## Data Types

![different types of containers](https://images.unsplash.com/photo-1589010588553-46e8e7c21788?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1260&q=80)

- ### Today we are going to discuss about Data Types in Arduino as we know how to use variables to store the important data inside those variables but we need to store the right data into right container.

- ### Let me tell you with example if we store Rice then we store it in a Rice container we can't contain rice inside sugar container beacuse it will mix both Rice and sugar and we will not get the result what we want and end up having lots of problems.

- ### You have seen how much variables are useful in previous blog but without specific data types variables efficiency decreases and we will not getting accurate results we wanted to achieve.

- ### If you want to learn more about Variables then read my previous blog link is given below :-

   [Variable](https://palashraghuwanshi.com/2022/introduction-to-arduino-03/)

- ### So learning Data types in Arduino or any other programming language like C, C++, Python, Java, Dart is quite useful to perform various operations easily so that we can get those accurate results and understand how computer thinks and work.

## Data Types in Arduino

![Different fruits in different boxes](https://images.unsplash.com/photo-1444459094717-a39f1e3e0903?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80)

- ### If we talk about Data Types in Arduino we can understand more easily by talking more and more real life situations as different types of Arduino boards are physical products and they are well associated with real life scenarios.

- ### Let me walk you though an example lets say if we want to store the pin numbers that will glow the led lights whose state is only HIGH or LOW so that they can switched ON and OFF or Blink according to our instructions is quite low in form of numbers so in that case we can use integer(int) data type as its capacity to store less in comparison of others.

- ### Another example of Data Types in Arduino is storing the temperature value coming from dht11 or dht22 or any other temperature sensor is float data type as it has the ability to store the numbers which are in floating point decimal numbers very well and we can easily store those floating point decimals coming from temperature sensor.

- ### Another pretty much good example of boolean data types is toggling the Leds with push button at different states as the boolean data type has only two state true or false which can be quite useful in toggle the two leds with push button by making one led true and it wil glow and at the same time making the other led false and it will stop glowing.

## Various Data Types in Arduino and its sizes and range

![Different size of parcels for different things](https://images.unsplash.com/photo-1624023749602-02bc0cda1278?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTJ8fHN0b3JhZ2V8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60)

- ### Boolean - Boolean data type  is only 1 byte in terms of size and it is ranges from 0 to 1 which can be only true or false as we have discussed earlier.

- ### char - char data type is only 1 byte in terms of size and it is ranges from -128 to 127.

- ### unsigned char - unsigned char data type is only 1 byte in terms of size and it is ranges from 0 to 255.Unsigned is basically used to get positive numbers.

- ### int - int data type is only 2 bytes in terms of size and it is ranges from  -32,768 to 32,767.

- ### unsigned int - unsigned int data type is only 2 bytes in terms of size and it is ranges from  0 to 65,535.Unsigned is basically used to get positive numbers.

- ### word - word data type is only 2 bytes in terms of size and it is ranges from  0 to 65,535.

- ### long - long data type is only 4 bytes in terms of size and it is ranges from  -2,147,483,648 to 2,147483,647.

- ### unsigned long - unsigned long data type is only 4 bytes in terms of size and it is ranges from  0 to 4,294,967,295.Unsigned is basically used to get positive numbers.

- ### float - float data type is only 4 bytes in terms of size and it is ranges from 3.4028235E-38 to 3.4028235E+38.

- ### double - double data type is only 4 bytes in terms of size and it is ranges from 	3.4028235E-38 to 3.4028235E+38.

- ### string - string data type is 1 byte + # of chars bytes in terms of size and it is ranges from N/A.

- ### Array - Array data type is 	1 byte + (sizeOfType * # of elements)  bytes in terms of size and it is ranges from N/A.

- ### We will discuss about Data Types and how we can use it in Arduino programming in my next Blog as if i will discuss in this blog it will become too lengthy.