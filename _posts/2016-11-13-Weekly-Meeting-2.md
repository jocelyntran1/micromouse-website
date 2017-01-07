---
layout: page
title: Weekly Meeting #2: Game Logistics and Block Diagram
---

#GAME LOGISTICS

* 16x 16 maze
* each team has ten minutes with the maze
* ten attempts total
* a cell is 180mm by 180mm

#BLOCK DIAGRAM

##MCU 
* control unit, stm32f4 (3.3v)
* turn emitters on/off

##POWER SUPPLY
* li-po battery (7.4v) 
* voltmeter (need way to read voltage of battery to keep li po battery above certain voltage)
* 5v linear drop out regulator (gives the circuit 5 v, dissipates the remaining 2.4v as heat)
* 3.3v linear drop out regulator

##INTERFACE
* buttons (3.3v) for switching between speed runs and searching runs
* LED (5v)

##SENSORS
* IR Emitters (5v)
* IR Recievers (3.3v)

##MOTOR CONTROL
* Level shifter
* H-Bridge (Used to control which side of the motor is powered, has extra protection (as opposed to using four switches, so we don't accidentally short the circuit and burn elements)
* Motors (7.4v)
* Encoders(5v) (keeps track of how much the motor has spun)


Microcontroller uses pwm to change the voltage going into motor to change speed
pulse width modulation - vary the width of the pulse to change the motor speed

Level shifter will bump up the 3.3v to 7.4v that goes into the motor since 3.3v is to little to power the motor