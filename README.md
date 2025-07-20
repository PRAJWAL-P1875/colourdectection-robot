🤖 Smart Line Follower with Color Detection and Servo Control
This Arduino-based project is a smart robot that combines line-following capability with color detection using the Adafruit TCS34725 color sensor. Based on the detected color (Red, Green, Blue), the robot performs specific actions like turning or moving forward, and additionally moves a servo motor for object interaction.

📌 Features
🔍 Line Following using two IR sensors (left and right)

🎨 Color Detection using Adafruit TCS34725 (Red, Green, Blue)

🔁 Dynamic Actions based on color:

🔴 Red: Move forward and operate servo

🟢 Green: Turn right and operate servo

🔵 Blue: Turn left and operate servo

⚙️ Servo Control for mechanical actions

💬 Serial feedback for monitoring and debugging

🛠️ Hardware Requirements
Component	Quantity
Arduino Uno / Mega	1
Adafruit Motor Shield v1/v2	1
TCS34725 Color Sensor	1
IR Sensors (Analog)	2
DC Motors	4
Servo Motor (SG90 recommended)	1
Jumper Wires	As needed
Power Supply (Battery/Adapter)	1

🔌 Circuit Connections
IR Sensors:
Left IR Sensor → A1

Right IR Sensor → A0

Motors (via Motor Shield):
Motor 1 → M1

Motor 2 → M2

Motor 3 → M3

Motor 4 → M4

Servo:
Signal → Digital Pin 9

TCS34725 Color Sensor:
SDA → A4 (on Uno) or appropriate I2C SDA

SCL → A5 (on Uno) or appropriate I2C SCL

VCC → 3.3V or 5V

GND → GND

📦 Installation & Setup
Install the following libraries in Arduino IDE:

Adafruit_TCS34725

AFMotor

Wire

Servo

Upload the code to your Arduino board using Arduino IDE.

Power the motor shield externally for best results.

🧠 Working Principle
Robot follows the line using two IR sensors.

When both sensors detect no line (off-track), it stops and activates color detection.

Based on the color:

🔴 Red: Moves forward and rotates the servo

🟢 Green: Turns right and rotates the servo

🔵 Blue: Turns left and rotates the servo

After the action, it resumes line-following mode.

📸 Demo
<img width="672" height="425" alt="Screenshot 2025-07-20 120920" src="https://github.com/user-attachments/assets/b6ad4141-f859-4ebd-9d41-7f9e27323fff" />


👨‍💻 Author
Prajwal .P
Electronics & Communication Engineer
IEEE Member | Embedded Systems Enthusiast | Robotics Developer

📄 License
This project is open-source and available under the MIT License.

