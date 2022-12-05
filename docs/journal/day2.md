# Journal - Day 2
Date: Tuesday, November 29, 2022

- Chose the Memory Game project, got it approved by the teacher
- Aritro started work on figuring out the wiring for the 8 bit shift register (75HC595)
  - The wiring for the shift register is somewhat complicated, so I (Aritro) worked on a TinkerCAD diagram before creating it in-person
  - I used [this article](https://lastminuteengineers.com/74hc595-shift-register-arduino-tutorial/) to understand more about it works 
- Byron and Haris started to work on wiring the rest of the components (LEDs, buttons, Arduino, buzzer, etc.)

## Pictures of Circuitry
Physical Circuit ![physical circuit](/media/pictures/pDay2.jpg))

## What is a shift register?
The shift register is an integrated circuit who's purpose is to store and transfer binary data. The circuit takes binary data as input from a microcontroller, and shifts each bit by one place for each presetted clock pulse and outputs the result through its output pins. 

As a powerful Arduino component, it consists of 16 pins: 3 of which are used as input pins and 8 used as output pins. This 8:3 ratio in terms of I/O pins reveals its ability to enhance circuit performance by reducing total tools used to complete a given task.

[source](https://electronicscoach.com/shift-register.html)
