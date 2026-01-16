# Blinking LED Using Arduino Uno 


## Project Information:
**Author:** Mohammed Kafil Ahmed
**Date:** 16 January 2026
**Platform:** Arduino Uno
**Simulation Tool:** Wokwi
**Programming Language:** Embedded C (Arduino) 

## Abstract: 
This project demonstrates basic digital output control using an Arduino Uno by blinking three LEDs in a predefined sequence. The experiment introduces fundamental concepts of embedded systems, including pin configuration, hardware interfacing, and timing control using software delays. 

## Objective:
To understand Arduino digital output operation 
To interface LEDs with an Arduino Uno 
To implement sequential LED blinking using software timing 

## Components Used: 
Arduino Uno 
Breadboard 
3 × LEDs (Red, Blue, Green) 
3 × Current-limiting resistors (220–330 Ω) 
Jumper wires 
USB cable 

## Circuit Description: 
Three LEDs are connected to Arduino digital pins 11, 12, and 13 through current-limiting resistors. The LED cathodes are connected to the Arduino GND. When a pin is set HIGH, the corresponding LED turns ON; when set LOW, it turns OFF. The breadboard is used for stable and organized connections. 

## Working Principle: 
The Arduino program configures the selected pins as outputs. Inside the loop() function, different combinations of HIGH and LOW signals are applied to the LEDs with defined delays. This creates a visible blinking and sequencing pattern that repeats continuously. 

## Source Code: 
void setup() { 
 pinMode(11, OUTPUT); 
 pinMode(12, OUTPUT); 
 pinMode(13, OUTPUT); 
} 
 
void loop() { 
 digitalWrite(11, HIGH); 
 digitalWrite(12, HIGH); 
 digitalWrite(13, LOW); 
 delay(1000); 
 
 digitalWrite(11, LOW); 
 digitalWrite(12, HIGH); 
 digitalWrite(13, HIGH); 
 delay(1000); 
 
 digitalWrite(11, HIGH); 
 digitalWrite(12, LOW); 
 digitalWrite(13, HIGH); 
 delay(1000); 
 
 digitalWrite(11, HIGH); 
 digitalWrite(12, LOW); 
 digitalWrite(13, LOW); 
 delay(500); 
 
 digitalWrite(11, LOW); 
 digitalWrite(12, HIGH); 
 digitalWrite(13, LOW); 
 delay(500); 
 
 digitalWrite(11, LOW); 
 digitalWrite(12, LOW); 
 digitalWrite(13, HIGH); 
 delay(500); 
} 
 
## Results:
LEDs blink in a defined and repeatable sequence 
Timing is controlled accurately using delay functions 
Circuit operates reliably without errors 

## Applications:
Basic Arduino and embedded systems learning 
LED indicators and signal systems 
Traffic light and animation simulations 

## Conclusion:
The blinking LED project was successfully implemented using Arduino Uno. It provides a solid foundation for understanding digital I/O control and embedded programming, serving as a reference for more advanced Arduino-based projects. 

## Future Improvements:
Replace delay() with timers 
Add push-button or sensor control 
Extend to traffic light or IoT applications 

## Circuit Diagram:
[Wokwi Circuit](Screenshot 2026-01-16 183725.png)    

## Wokwi Simulation:
Wokwi Project Link: https://wokwi.com/projects/453306385466180609 

