---
layout: project
type: project
image: images/HIIT.jpg
title: HIITicker
permalink: projects/micromouse
# All dates must be YYYY-MM-DD format!
date: 2021-12-28
labels:
  - iOS
  - Swift
  - SwiftUI
summary: I developed a HIIT timing and guidance app for iOS & watchOS
---

<div class="ui small rounded images">
  <img class="ui image" src="../images/HIIT.jpg">
  <img class="ui image" src="../images/HIIT2.jpg">
</div>

HIITicker is an app I developed to aid in High Intensity Interval Training routines.

For this project, I was the lead programmer who was responsible for programming the various capabilities of the mouse.  I started by programming the basics, such as sensor polling and motor actuation using interrupts.  From there, I then programmed the basic PD controls for the motors of the mouse.  The PD control the drive so that the mouse would stay centered while traversing the maze and keep the mouse driving straight.  I also programmed basic algorithms used to solve the maze such as a right wall hugger and a left wall hugger algorithm.  From there I worked on a flood-fill algorithm to help the mouse track where it is in the maze, and to map the route it takes.  We finished with the fastest mouse who finished the maze within our college.

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
```

You can learn more at the [UH Micromouse Website](http://www-ee.eng.hawaii.edu/~mmouse/about.html).



