# Ultrasonic-digital-sensor-
This Arduino project uses an ultrasonic sensor to detect the distance of nearby objects. Based on the distance, it turns on one of three LEDs (red, yellow, green) and optionally activates a buzzer to signal when something is too close.
_________________________________________________________________________
 Hardware Components:

Arduino UNO

Ultrasonic sensor (HC-SR04)

3 LEDs: Red, Yellow, Green

3 Resistors (220Ω) for LEDs

1 Buzzer (passive)

Breadboard

Jumper wires
____________________________________________________________________________
 Wiring Connections:
 Ultrasonic Sensor (HC-SR04):
Pin	Connected to Arduino
VCC	5V
GND	GND
Trig	D6
Echo	D5
_____________________________________________________________________________
 LEDs:
Color	Arduino Pin	Notes

Green	D10	Far = Green ON

Yellow	D9	Medium = Yellow ON

Red	D8	Close = Red ON

Each LED connects through a 220Ω resistor to ground.
______________________________________________________________________________
 Buzzer:
Buzzer Pin	Connected to Arduino
+ (long leg)	D7
– (short leg)	GND
_______________________________________________________________________________
 How the Project Works:
The ultrasonic sensor sends out a sound pulse and listens for it to bounce back.

The Arduino calculates the distance using the time it takes for the echo.
_______________________________________________________________________________
Based on the distance:

🔴 If distance < 20 cm → Red LED ON, buzzer beeps.

🟡 If 20–40 cm → Yellow LED ON, no buzzer.

🟢 If > 40 cm → Green LED ON, no buzzer.
_______________________________________________________________________________
Project Applications:
Smart parking sensors

Object detection for robots

Safety proximity alerts

Distance-based lighting or signaling
_________________________________________________________________________________

<img width="1265" height="736" alt="‪Circuit design UltraSonic (digital) - Tinkercad - Google Chrome‬ 20_01_47 10_37_12 م" src="https://github.com/user-attachments/assets/ea70f1e3-b4ba-4d52-9f46-1591d664a570" />



