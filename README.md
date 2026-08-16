# IoT-Enabled Smoke Detection System Using Arduino

## Aim

To design, simulate, and analyze an IoT-enabled Smoke Detection System using Arduino Uno in Proteus Professional, which detects smoke concentration using an MQ-2 gas sensor and sends alert information through a simulated IoT communication module while activating visual and audible alarms.

## Apparatus Required

**S. No	Components/Software	Specification	Quantity**
1	Arduino Uno	ATmega328P	1
2	MQ-2 Smoke/Gas Sensor	Analog Output	1
3	ESP8266 Wi-Fi Module (Virtual) / Virtual Terminal	IoT Communication	1
4	LED	Red	1
5	Buzzer	5V Active Buzzer	1
6	Resistor	220 Ω	1
7	Potentiometer (Optional)	For sensor simulation	1
8	Virtual Terminal	Display sensor data	1
9	Proteus Professional Software	Version 8 or above	1
10	Arduino IDE	Program Development	1
11	Connecting Wires	Virtual	As required

## Procedure

Step 1: Create the Circuit
Open Proteus Professional.
Create a new project.
Place the following components:
Arduino Uno
MQ-2 Gas Sensor (or variable analog source for simulation)
ESP8266 (or Virtual Terminal)
LED
Buzzer
220 Ω resistor

Step 2: Make Circuit Connections
Connect the MQ-2 sensor analog output to A0 of Arduino.
Connect LED to Digital Pin 8 through a 220 Ω resistor.
Connect buzzer to Digital Pin 9.
Connect ESP8266 TX/RX (or Virtual Terminal) to Arduino Serial communication pins.
Connect all VCC and GND terminals appropriately.

Step 3: Develop Arduino Program
Open Arduino IDE.
Write the program to:
Read MQ-2 sensor values.
Compare the sensor value with a predefined threshold.
Turn ON LED and buzzer when smoke exceeds the threshold.
Send smoke level and alert message through Serial communication (IoT simulation).

Step 4: Generate HEX File
Verify and compile the program.
Generate the Arduino HEX file.
Load the HEX file into the Arduino Uno in Proteus.

Step 5: Run the Simulation
Start the Proteus simulation.
Increase the MQ-2 sensor value using the sensor control or variable voltage source.

Observe:
Smoke sensor readings
LED status
Buzzer operation
Alert message in Virtual Terminal

Step 6: Analyze the Output

Verify that:
Normal condition displays safe smoke levels.
High smoke concentration activates LED and buzzer.
Alert message is transmitted via the simulated IoT interface.

## Circuit Diagram & OUTPUT


<img width="1916" height="1140" alt="image" src="https://github.com/user-attachments/assets/439c754a-9e6d-4e12-afa6-19e942629856" />





## Result

The IoT-enabled Smoke Detection System was successfully designed and simulated using Proteus. The Arduino continuously monitored smoke concentration from the MQ-2 sensor. When the smoke level exceeded the predefined threshold, the system successfully activated the LED and buzzer and transmitted an alert message through the simulated IoT communication interface. The experiment demonstrated the effective implementation of a smart smoke monitoring and early warning system suitable for home, office, and industrial safety applications.
