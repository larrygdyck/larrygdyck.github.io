---
layout: project
type: project
image: images/output.png
title: Appelbrot
permalink: projects/vacay
# All dates must be YYYY-MM-DD format!
date: 2021-12-15
labels:
  - Swift
  - SwiftUI
  - Metal
  - GitHub
summary: A macOS fractal screensaver
---

<img class="ui medium right floated rounded image" src="../images/output.png">

Appelbrot is a macOS application/screensaver that I created as a demonstration of Metal performance capabilities. The project helped me learn how to use the GPU to accelerate algorithms that are able to operate in parallel and to implement a novel screensaver in the process.

Here is some code that illustrates how we read values from the line sensors:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}

In this project I gained experience with full-stack web application design and associated technologies, including [MongoDB](http://mongodb.com) for database storage, the [Twitter Bootstrap](http://getbootstrap.com/) CSS Framework for the user interface, and Javascript for both client and server-side programming. 
 
Source: <a href="https://github.com/theVacay/vacay"><i class="large github icon"></i>theVacay/vacay</a>
