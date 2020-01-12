# Ultrasonic-Rangefinder-using-8051

## Gautam Mishra
- Supervisior : Dr. Prashanth G.R
- Microprocessor and Microcontroller Laboratory
- Department of Computer Science and Engineering
- November 23, 2019


## Objective
- The objective of this experiment is to built a Ultrasonic rangefinder using 8051 Microcontroller and Ultrasonic Sensor which measures the distance up to 4 meters.

## Requirements
- 8051 Microcontroller
- 16X2 LCD Unit
- HC-SR04 Ultrasonic Sensor
- Jumper wires

###  Software Requirements
- Keil Uvision 3
- Programming language: C Language

## Introduction
#### Principle of Ultrasonic Rangefinder
- Generally, the distance can be measured using pulse echo method. The ultrasonic module
transmits a signal to the object, then receives echo signal from the object and produces output
signal whose time period is proportional to the distance of the object. The mechanism of the
ultra sonic sensor is similar to the RADAR (Radio Detection and Ranging).  

This circuit calculates the distance of the object based on the speed of the sound wave at normal temperature and displays the distance on LCD.  

#### How Ultrasonic Rangefinder using 8051 Circuit works?
1. The HC-SR04 module has ultrasonic transmitter, receiver and control circuit on a singleboard.  The module has only 4 pins, Vcc, Gnd, Trig and Echo.
2.  When a pulse of 10sec or more is given to the Trig pin, 8 pulses of 40 kHz are generated.After this, the Echo pin is made high by the control circuit in the module.
3.  Echo pin remains high till it gets echo signal of the transmitted pulses back.
4.  The time for which the echo pin remains high, i.e.  the width of the Echo pin gives thetime taken for generated ultrasonic sound to travel towards the object and return.
5.  Using this time and the speed of sound in air, we can find the distance of the objectusing a simple formula for distance using speed and time.

### Ultrasonic Module (Ultrasonic Sensor)
HC SR04 Ultrasonic Module works on the principle of SONAR and is designed to measure therange of the object in small embedded projects.  It offers excellent range detection with highaccuracy and stable readings.  The operation of the module is not affected by the sunlight orblack material.

### To measure distance
1.  Object Distance(in cm) = (Sound Velocity * Time)/2,Where, Sound Velocity = 34300 (in cm per second)
2.  Here, oscillator frequency of AT89S52 (8051) is 11.0592 MHz, then timer frequency of8051 will be 921.6 kHz.
3.  So, Time required to execute 1 instruction is 1.085 us.
4.  So, timer gets incremented after 1.085 us time elapse.

### Procedure
1.  Initially burn the program to the microcontroller  
2.  Now give the connections as per the circuit diagram  
3.  While giving the connections make sure that Vcc of ultrasonic module is connected to5V DC  
4.  Switch on the board supply  
5.  Place the obstacle in front the ultrasonic module, now you can observe the distance onLCD.  
6.  Switch off the board supply  

### Result  
Using the mechanism of ultrasonic sensor, Interfacing of Ultrasonic module HC-SR04 with8051 Microcontroller was performed successfully and by moving the object to and fro towardsultrasonic module the distance up to 4 meters was measured correctly
