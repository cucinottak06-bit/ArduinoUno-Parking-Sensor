# Arduino Parking Sensor

## Overview

This project is an Arduino-based parking sensor that uses an ultrasonic sensor to detect the distance between the sensor and a nearby object. The measured distance is displayed on a 16x2 LCD, while a buzzer provides an audible warning as an object approaches.

I expanded the original parking sensor design by adding green, yellow, and red LEDs to provide a visual indication of how close an object is to the sensor simulating  a modern back up camera.

## Features

- Real-time distance measurement using an ultrasonic sensor
- 16x2 LCD distance display
- Green, yellow, and red LED proximity indicators
- Audible warning using a buzzer
- Different warnings based on object distance

## Components

- Arduino Uno
- HC-SR04 Ultrasonic Sensor
- 16x2 LCD
- Green LED
- Yellow LED
- Red LED
- Buzzer
- Resistors
- Breadboard
- Jumper wires
- USB cable/power source

## How It Works

The HC-SR04 ultrasonic sensor sends an ultrasonic pulse toward an object and measures how long it takes for the reflected signal to return.

The Arduino uses this time to calculate the distance:

Distance = (Time x Speed of Sound) / 2

The calculated distance is displayed on the LCD.

The LEDs provide an additional visual warning:

- Far: Green LED
- Medium: Yellow LED
- Close: Red LED

As an object approaches the sensor, the system changes the LED indicator and uses the buzzer to warn the user.

## Schematic

![Parking Sensor Schematic](images/schematic.png)

## Final Build

![Completed Arduino Parking Sensor](images/final_project.jpg)

## Testing and Results

The system was tested by placing objects at different distances in front of the ultrasonic sensor.

- Object far from sensor: Green LED activates - Pass
- Object at medium distance: Yellow LED activates - Pass
- Object close to sensor: Red LED activates - Pass
- Object distance changes: LCD updates measured distance - Pass
- Object approaches sensor: Audible warning activates/changes - Pass

Testing confirmed that the system could detect changes in object distance and provide visual and audible proximity feedback.

## Skills Demonstrated

- Arduino programming
- C/C++
- Ultrasonic distance measurement
- Sensor interfacing
- LCD interfacing
- Digital outputs
- Circuit prototyping
- Breadboard wiring
- Hardware troubleshooting
- System testing

## Project Files

- parking_sensor.ino - Arduino source code
- images/final_project.jpg - Photo of the completed project
- images/schematic.png - Circuit schematic

## Credits

This project was based on the Parking Sensor project by Jackaless on Arduino Project Hub:

https://projecthub.arduino.cc/jackaless/parking-sensor-4aa9d0

I modified and expanded the project by adding LED proximity indicators and integrating them into the parking sensor system.
