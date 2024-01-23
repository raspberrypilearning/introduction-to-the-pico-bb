## Introduction
This guide shows you how to connect a Raspberry Pi Pico to another computer and program it using the `picozero` beginner library with MicroPython.

### What is the Raspberry Pi Pico?
A Raspberry Pi Pico is a low-cost microcontroller device. Microcontrollers are tiny computers, but they tend to lack large volume storage and peripheral devices that you can plug in (for example, keyboards or monitors).

A Raspberry Pi Pico has GPIO pins, much like a Raspberry Pi computer, which means it can be used to control and receive input from a variety of electronic devices.

![Image of the small Pico board being held in a hand.](images/pico-hand.png)

--- collapse ---
---
title: What you will need
---
### Hardware

+ A Raspberry Pi Pico with soldered headers
+ A computer that can run the Thonny IDE and program a Raspberry Pi Pico
+ A micro USB data cable
+ An external 5V micro USB power source (optional) 

To complete the [Introduction to Raspberry Pi Pico](https://projects.raspberrypi.org/en/pathways/pico-intro) path:

+ 1 red LED
+ 1 yellow LED
+ A selection of other single-colour LEDs
+ At least one **common cathode** RGB LED
+ At least one potentiometer
+ At least one passive buzzer
+ At least four push buttons
+ 100Ω resistors (any resistor from 75Ω-220Ω will work) 3 per RGB LED, 1 per single colour LED
+ A selection of socket-to-socket jumper leads and socket-pin jumper leads.

When purchasing jumper wires you may notice that they are called male-male (m-m), female-female (f-f) and male-female (m-f). This is legacy (prior) language used to describe the ends of the wires. Pin and socket are more inclusive terms that should now be used to describe jumper wires.

**Note:** You can reuse components in multiple projects. If you have additional components then you won't have to take each project apart to make the next one. 

### Software

The project will guide you through the installation of:
 
+ The Thonny Python IDE
+ MicroPython firmware for Raspberry Pi Pico
+ The picozero library

--- /collapse ---

### How to use this reference guide

If you have not used a Raspberry Pi Pico before, then this guide will help you to get set up and create your first program. Then you will be ready to start the [Introduction to Raspberry Pi Pico](https://projects.raspberrypi.org/en/pathways/pico-intro) path.

You can return to this guide and use it to look up information that you need when you are making your own projects with the Raspberry Pi Pico.

**Note:** Advanced MicroPython users can use [Getting Started with Raspberry Pi Pico](https://projects.raspberrypi.org/en/projects/getting-started-with-the-pico). 