# Strategy for Our Robot in Gameplay

At the start of the game, the robot utilizes a balance sensor (Gyro) to reset its balance, ensuring stability while walking forward and turning. It employs three ultrasonic sensors located at the front to prevent collisions with walls or columns. When these sensors detect the robot moving away from a wall, they send commands to the Arduino to adjust its distance appropriately.

When the robot detects a blue line, the HuskyLens sends a command to the Arduino to move forward and then turn 60 degrees to the left, continuously repeating this process. Simultaneously, as the HuskyLens identifies the blue line, a Pixy camera mounted on a servo turns left to detect the color of the column on that side.

If the Pixy camera encounters a green column, it instructs the Arduino to turn left to navigate along the left side of the column. Conversely, if it detects a red column, it commands the robot to move forward a safe distance before turning right to follow the right side of the red column. This method continues until the robot completes three rounds, reading all blue lines three times before stopping at its starting point.

#Using the Arduino Mega 2560
We program the Arduino Mega using the Arduino IDE. To begin, we need to install the Arduino IDE software. Alternatively, we can use the Arduino Web Editor, which allows sketch uploads and code writing directly from a web browser (Google Chrome is recommended). The USB cable is essential for connecting the board to the computer, indicated by the green LED lighting up, confirming a successful connection.

##Steps to Get Started with Arduino Mega
Open the code or sketch in the Arduino software.
Select the board type.
Choose the ATmega2560 microcontroller for the Arduino Mega, which is automatically selected by default.
For further details on using the Arduino, visit the Arduino Mega Guide.

## The Program
All of our source codes are located in the src directory.

## Components of the Robot
### Arduino Mega 2560

- The Arduino Mega 2560 is a development board based on the Atmega2560 microcontroller, ideal for projects requiring more GPIO pins and memory. It features 16 analog pins and 54 digital I/O pins, with 15 serving as PWM outputs.
### HuskyLens

- The HuskyLens is a vision sensor with seven built-in functions, including object tracking and line tracking. It connects via UART/I2C to the Arduino, allowing the robot to identify pillars on the game board.
### 3D Printer

- We designed the robot using Autodesk Inventor and printed parts with a 3D printer, including the cover and sensor boxes.
### DC Motor

- DC motors allow the robot to move forward and backward, powered by direct current.
### Servo

- Servos provide precise control of angular position and are used to move the wheels and camera.
### L298N Motor Driver

- The L298N driver controls the direction and speed of two DC motors using H-Bridge and PWM techniques.
### Pixy Camera

-The Pixy camera is a complete vision system that detects colors and lines, essential for navigation.
### Gyro Sensor (MPU6050)

-The MPU6050 sensor integrates a 3-axis accelerometer and gyroscope for measuring motion and orientation.
### Laser Cutter Machine

- We used a laser cutter to create precise parts, such as engine gears.
### RPLIDAR

-The RPLIDAR A1 is a low-cost 360-degree laser scanner for mapping and localization.

### Ultrasonic Sensor (HC-SR04)

-We utilized ultrasonic sensors to help the robot avoid obstacles and maintain a safe distance.
### Batteries

- We used four batteries to provide a total of 12 volts.
  
### Voltage Regulator

- The voltage regulator maintains a stable output voltage for the robot's components.
### Switches

- The robot includes two switches: one to power it on and off, and another to start the game.
For any further details or inquiries, feel free to reach out!

# (Time has betrayed us, but we will succeed in the end, God willing.)


