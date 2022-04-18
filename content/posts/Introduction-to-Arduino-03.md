---
categories: ["Arduino"]
description: Arduino Tutorial for beginners to build the innovative products and use it in our daily life
author:
  name : "Peelu"
date: "2022-04-15"
linktitle: "Introduction to Arduino Programming-01"
type: 
  - post
  - posts
title : "Introduction to Arduino Programming-01"
tags: ['arduino','innovation']
featured_image: https://images.unsplash.com/photo-1553406830-ef2513450d76?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1031&q=80
weight : 10
series:  
  - Hugo 101
---

## Introduction

![Honey stored in a container like we contain leds inside a variable](https://cdn.pixabay.com/photo/2015/06/27/16/35/honey-823614_960_720.jpg)

- ### Before we start our Tutorial my humble request is to use simulation softwares like Tinker Cad, Wokwi and Proteus as much as possible at the time of learning because nowadays we all are facing climate change, global-warming etc and we need to use less hardwares atleast at the time of learning or building the prototypes.

- ### Learning Arduino without learning Programming is like a Magician without his or her Magical instruments.

- ### In order to innovate the magical products we need to understand the basic fundamentals of Programming like variables, data-types, functions, loops like for loops, while loops and do while loops etc

- ### We will start our journey of Arduino Programming by learning variables and its uses in Arduino.

- ## Variables

- ### Variables are nothing but a container to store some data for a later use. You can think like a Bag full of Books or School full of students and teachers etc.

- ### Variables are quite useful in Arduino as we can store our different Digital and Analog pins or pin numbers inside our Variable and use it whenever we need them and even changed it whenever we changed the pin number.

- ### Variables reduces our code by storing Different pin numbers and makes our code more meaningful so that we and other humans can understand our and others code well.

- ## Let me walk you through ours real world scenarios of our daily life:-

![Light bulb pins stored in a container](https://images.unsplash.com/photo-1623780569981-8ecf6b181928?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1118&q=80)

- ### When you see a light buld inside your room , that is powered on and off according to our needs and wants whenever we pressed the ON switch, the light bulb will glow and shine and whenever we pressed the OFF switch the light bulb will stop glowing.

- ### If we want to control that light bulb with our Arduino or other Micro - Controllers available in the market like powering on and off with our mobile phones then we need to store that Light Bulb pin number in Variable and use it whenever we need according to our instructions and desires isn't it amazing the working process of variable we can control our home appliances.

- ### When you see those fans inside your rooms giving you cool Air whenever you feels warm, those are powered on and off according to our needs and wants whenever we pressed the ON Button, the Fan will turn ON and gives us cool air stored in form of electricity and whenever we pressed the OFF Button the Fan will turn OFF and stop giving Air.

- ### If we want to control those Fan with our Arduino or other Micro - Controllers available in the market like powering on and off with our voice instructions then we need to store those Fan pin number in Variable and control our room Fan according to our voice commands.

## Web-Development vs Arduino Variables

![Web Designs](https://images.unsplash.com/photo-1547658719-da2b51169166?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=464&q=80)

- ### Even though all variables are same whether you use in Web Development, Android Development, BlockChain or any other Development but when it comes to understanding of the real world philosophy of variables, you can understand better by innovating different Arduino projects and you will surely feel like real world scenarios.

- ### In web development you will use variables in building those cool designs or storing data in Backend API but in Arduino you can store physical products inside your variables like LEDs, motors, various kinds of sensors and the list will never end.

![innovations](https://images.unsplash.com/photo-1485827404703-89b55fcc595e?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80)

- ### In web development you have a oppurtunity of high paying salary but in Arduino projects you have a opportunity to innovate something for the needy ones and give back to the society.

- ### After all these are my opinions every field has its own limitations and advantages regardless what you enjoy, to be honest I am feeling those wow moments whenever I am learning Arduino or other embedded development stuff.

## How to use Variables in Arduino

- ### There are two types of variables in Arduino:-

- ## Local Variables :- Variables that are declared inside a function or block are local variables. They can be used only by the statements that are inside that function or block of code. Local variables are not known to function outside their own. Following is the example using local variables −

## How to use Local Variables in Arduino

- ### Void setup () {

- ### }

- ### Void loop () {

- ###    int x , y; // local variable declared inside the function and can be used in this function only

- ###    int z ; Local variable declaration

- ###    x = 0;

- ###    y = 0; actual initialization

- ###    z = 10;

- ### }


- ## Global Variables :- Variables that are created outside of a function are known as global variables.Global variables can be used by everyone, both inside of functions and outside.

## How to use Global Variables in Arduino

- ### int ledPin = 13; // Global variable  declared outside the function and can be used anywhere in the program

- ### Void setup () {

- ### pinMode(ledPin,OUTPUT);

- ### }

- ### Void loop () {

- ### digitalWrite(ledPin,HIGH)

- ### delay(300); //300 milliseconds

- ### digitalWrite(ledPin,LOW)

- ### delay(300); //300 milliseconds

- ### }


