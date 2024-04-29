# Two-Way Traffic Signal Arduino Project
Link to Tinkercad simulation - https://www.tinkercad.com/things/9TXUvdl8Ojz-2-way-traffic-light?sharecode=YUjy9RwIrkLmc8MBtxo399pwvaGYzw-9APE-YyD8ACk
## Overview
This Arduino project simulates a two-way traffic signal system using LEDs to represent the traffic lights. The system consists of two sets of traffic lights, each controlling traffic flow in opposite directions.

### Components
- Arduino board - Arduino Uno R3
- LEDs (Red, Yellow, Green) for each traffic light
- 6 220ohm Resistors
- Breadboard
- Jumper wires

### Code Explanation
#### Variable Declarations
Declares pin numbers for each LED corresponding to both sets of traffic lights.
#### Setup Function
Initializes the pins as output pins for each LED.
#### Loop Function
Calls the changeLights() function to alternate between different states of the traffic lights with a delay of 10 seconds between each change.
#### ChangeLights Function
Defines the logic for changing the traffic lights according to the traffic signal sequence:
1. Both yellow lights turn on for 3 seconds.
2. Red1 and Green2 lights turn on while yellow lights turn off for 7 seconds.
3. Both yellow lights turn on for 3 seconds.
4. Green1 and Red2 lights turn on while yellow lights turn off for 7 seconds.

