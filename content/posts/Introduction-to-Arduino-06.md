---
categories: ["Arduino"]
description: Arduino Tutorial for beginners to build the innovative products for the needy ones and use it in our daily life
author:
  name : "Peelu"
date: "2022-04-21"
linktitle: "Introduction to Arduino-06"
type: 
  - post
  - posts
title : "Introduction to Arduino-06"
tags: ['arduino','innovation']
featured_image: https://images.unsplash.com/photo-1635186646209-962eddb4d094?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1171&q=80
weight : 10
series:  
  - Hugo 101
---

## Introduction

- ### Before we start our Tutorial my humble request is to use simulation softwares like Tinker Cad, Wokwi and Proteus as much as possible at the time of learning because nowadays we all are facing climate change, global-warming etc and we need to use less hardwares atleast at the time of learning or building the prototypes.

- ### So today we will discuss more about other data types in Arduino Programming which can be used to create magical products according to our imagination and thinking abilities.

- ### Every day  I am learning and sharing what I am learning and when i see those magical and innovative projects from the experienced and people in this field, i feel oh there is no limit of how we think we can create whatever we want.

- ### I think so I and we all can create those out of the box, innovative projects if we all continue to learn those small amount of knowledge each and every single day with fun and excitement.

- ### So let's start our today's lesson with boolean data type

## Bool :- Bool or Boolean data type is quite important when it comes to switch between two states either true or false and can make our program too easy if we have to deal with true and false only.

![Toggle Leds](https://images.unsplash.com/photo-1527356900876-cae61d8d8462?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1176&q=80)

  - ### Let me walk you through with an example lets imagine if we want to toggle the two leds with push button switch means when we press and release the push button first then led1 will ON and led2 will OFF and if we push again then led2 will ON and led1 will OFF.

  - ### Now we will see how to toogle the two Leds and with push button with the help of Boolean Data type, you can easily program in any simulation softwares like Tinker Cad, Wokwi or Proteus.

  - ### // #define which is used as a constant and did not take any memory on the chip
  - ### #define led1 11 // first we have defined our led1 pin number with #define 
  - ### #define led2 10 // second we have defined our led2 pin number with #define 
  - ### #define BUTTON_PIN 2 // third we have defined our push button pin number with #define 

  - ### int toggleLedState = 1; // fourth we have made the variable with the help of int so that we can change afterwards accordingly
  - ### // unsigned keyword is used to make our variable positive from -2,147,483,648 to 2,147483,647 to 0 to 4,294,967,295.
  - ### unsigned long lastTimeButtonChange = millis(); // 5th we have made variable with unsigned long 
  - ### unsigned long debounceDelay = 50;
  - ### byte buttonState =  LOW; // 6th we have made the boolean variable with byte so that it will take less memory on arduino chip

  - ### Then we have made a toggle led function which we will use in void loop
  - ### void toggleOtherLeds()
  - ### {
  - ### // whenever we push the push button for the first time led2 will ON and led1 will OFF and next time led1 will ON and led2 will OFF
  - ### if(toggleLedState == 1){
    - ### toggleLedState = 2;
    - ### digitalWrite(led1,LOW);
    - ### digitalWrite(led2,HIGH);
  - ### }
  - ### else
  - ### {
   	- ### toggleLedState = 1;
    - ### digitalWrite(led1,HIGH);
    - ### digitalWrite(led2,LOW);
        - ### }
    - ### }

    - ### void setup()
- ### {
  - ### pinMode(led1, OUTPUT);
  - ### pinMode(led2, OUTPUT);
  - ### pinMode(BUTTON_PIN,INPUT);
  - ### buttonState = digitalRead(BUTTON_PIN);
- ### }
    
- ### void loop()
- ### {
- ### // Then we have taken current time with millis() and stored in timeNow variable
  - ### unsigned long timeNow = millis(); //current time
  - ### // toggle led 2 and 3 when the button is pressed
  - ### if(timeNow - lastTimeButtonChange > debounceDelay){
    - ### byte newButtonState = digitalRead(BUTTON_PIN);
    - ### if(newButtonState != buttonState){
      - ### lastTimeButtonChange = timeNow;
      - ### buttonState = newButtonState;
      - ### if(buttonState == HIGH){
       - ### toggleOtherLeds(); 
      - ### }
    - ### }
  - ### }

- ### }

## String :- String data type is very important when it comes to print something on the Serial Monitor or lcd screen or any other screen as we can easily store String values inside it.

   - ### Let me explain you with quick example lets say if we want to advertise our shop name on the lcd screen we can easily do it with String data type.

   ![Advertise your products with LCD](https://images.unsplash.com/photo-1622988766425-8ecbae9cef6c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80)
   
   - ### Now we will see how to print something on the lcd screen with scrolling with the help of Boolean Data type, you can easily program in any simulation softwares like Tinker Cad, Wokwi or Proteus.

   - ### #include <LiquidCrystal.h> //lcd library
   - ### LiquidCrystal lcd(13,12,11,10,9,8); // these pins are connected to lcd

   - ### void setup() 
   - ### {

  - ### // put your setup code here, to run once:
  - ### // We have tell our compiler that we are using 16x2 lcd with lcd.begin function
  - ### lcd.begin(16,2);
   - ### }

   - ### void loop()
   - ### {

  - ### // put your main code here, to run repeatedly:
  - ### lcd.setCursor(0,0); // column first then row
  - ### String msg1 = "Raghuwanshi Tyres"; // typed our first message with String data type and you can change accordingly your own choice
  - ### lcd.print(msg1); // print our first message on lcd screen at (0,0) position
  - ### delay(500); // then we have given delay of half second so that it will stop some time before scrolling
  - ### then we have used a for loop so we can scroll each and every single character
  - ### for(int pos = 0; pos < msg1.length(); pos++)
  - ### {
    - ### lcd.scrollDisplayLeft(); //scrolling left with lcd.scrollDisplayLeft(); function and you can scroll write with lcd.scrollDisplayRight();
    - ### delay(200);
  - ### }
  - ### lcd.clear(); // then we have cleared our screen so that next message will be printed
  - ### lcd.setCursor(0,1); // column first then row
  - ### String msg2 = "Raghuwanshi Collection"; //2nd message
  - ### lcd.print(msg2); // print our second message on lcd screen at (0,1) position
  - ### delay(500);
  - ### for(int pos = 0; pos < msg2.length(); pos++)
  - ### {
    - ### lcd.scrollDisplayLeft(); //scrolling left with lcd.scrollDisplayLeft(); function and you can scroll write with lcd.scrollDisplayRight();
    - ### delay(200);
  - ### }
  - ### lcd.clear();  // then we have cleared our screen so that next message will be printed

  - ### }


  


