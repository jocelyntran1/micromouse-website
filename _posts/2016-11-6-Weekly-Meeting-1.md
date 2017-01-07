---
layout: page
title: Weekly Meeting #1: Circuit Board Design
---

# Circuit Designs
Started making schematics on Eagle
Designed led receiver circuit and led emitter circuit

# Capacitors?
Discussed the need of capacitor in the circuit
Pro: noise reduction 
Con: doesn't turn off immediately

# Sensors
To gather sensor values, we must turn on an led one at a time, read the value, turn it off, and repeat with the other LEDs. If we turn more than one LED on at once, we may get inaccurate readings because of interference. If we keep an LED on for too long, it might burn out. 

# Darlington Array
We will use darlinton array which has 7 switches. This will turn on/off each LED separately.