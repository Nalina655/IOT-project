LED Control via Arduino and Bluetooth Module
📖 Overview

This project demonstrates a wireless LED control system that allows users to remotely toggle lights using a smartphone or any Bluetooth-enabled device. It showcases the integration of embedded systems and IoT-based communication through Arduino and the HC-05 Bluetooth module.

By establishing a serial communication link between the Bluetooth module and Arduino, users can send commands (such as ON and OFF) to control an LED in real-time — representing a simple yet powerful concept of wireless device control.

⚙️ Features

🔹 Wireless LED control via Bluetooth

🔹 Real-time communication between mobile device and Arduino

🔹 Simple command-based control (ON/OFF)

🔹 Demonstrates embedded system & IoT fundamentals

🧠 Working Principle

The HC-05 Bluetooth module pairs with a smartphone using any Bluetooth terminal app.

The Arduino Uno receives serial commands from the module.

Based on the command (ON or OFF), the Arduino toggles the LED’s state.

🧰 Tools & Technologies

Hardware: Arduino Uno, HC-05 Bluetooth Module, LED, Resistor (220Ω), Jumper Wires

Software: Arduino IDE

Programming Language: C/C++ (Arduino)

🪜 Circuit Connections
Component	Arduino Pin	Description
HC-05 TX	D2 (SoftwareSerial RX)	Receives data from Bluetooth
HC-05 RX	D3 (SoftwareSerial TX)	Sends data to Bluetooth
LED (+)	D13	LED positive terminal
LED (–)	GND	LED ground connection
HC-05 VCC	5V	Power supply
HC-05 GND	GND	Ground


📱 How to Use

Upload the code to your Arduino Uno.

Power up the HC-05 module and pair it with your phone (default PIN: 1234 or 0000).

Open any Bluetooth Terminal App (e.g., Bluetooth Terminal HC-05 on Android).

Send:

1 → Turn ON LED

0 → Turn OFF LED

🔋 Applications

Smart home lighting systems

IoT-based automation projects

Remote device control prototypes

