# Smart Parking Slot Availability and Warning System
An Arduino-based embedded system that monitors a single parking slot
using an ultrasonic sensor with real-time LED feedback and overtime alerts.

## Features
- Real-time occupancy detection (HC-SR04 ultrasonic sensor)
- Green LED when slot is free, Red LED when occupied
- Alert LED for overtime parking beyond configurable threshold
- Serial Monitor live status logging
- Fully configurable distance threshold and alert timer
- Fully commented beginner-friendly code

## Quick Start (Tinkercad)
1. Open tinkercad.com and create a new Circuit
2. Place and wire components per the circuit table
3. Paste smart_parking.ino into the Code editor (Text mode)
4. Click Start Simulation and test with the sensor slider

## Expected Outputs
Slot Free    : Green ON | Red OFF | Alert OFF
Slot Occupied: Green OFF | Red ON  | Alert OFF
Overtime     : Green OFF | Red ON  | Alert ON

## Configuration
const int DISTANCE_THRESHOLD = 20;
const unsigned long ALERT_THRESHOLD_MS = 10000;
