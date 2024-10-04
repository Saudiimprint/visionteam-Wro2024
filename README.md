
<img src="=https://cdn.discordapp.com/attachments/1070762024700739585/1290342723475214407/welcome_to_our_Web_1.png?ex=6700ba0e&is=66ff688e&hm=df486755d818874074346f6dd20563b9c80539434547cb58d2e70b7f6ee54856&;&center=true&size=25">



# Strategy for Our Robot in Gameplay

At the start of the game, the robot utilizes a balance sensor (Gyro) to reset its balance, ensuring stability while walking forward and turning. It employs three ultrasonic sensors located at the front to prevent collisions with walls or columns. When these sensors detect the robot moving away from a wall, they send commands to the Arduino to adjust its distance appropriately.

When the robot detects a blue line, the HuskyLens sends a command to the Arduino to move forward and then turn 60 degrees to the left, continuously repeating this process. Simultaneously, as the HuskyLens identifies the blue line, a Pixy camera mounted on a servo turns left to detect the color of the column on that side.

If the Pixy camera encounters a green column, it instructs the Arduino to turn left to navigate along the left side of the column. Conversely, if it detects a red column, it commands the robot to move forward a safe distance before turning right to follow the right side of the red column. This method continues until the robot completes three rounds, reading all blue lines three times before stopping at its starting point.

# Using the Arduino Mega 2560

We program the Arduino Mega using the Arduino IDE. To begin, we need to install the Arduino IDE software. Alternatively, we can use the Arduino Web Editor, which allows sketch uploads and code writing directly from a web browser (Google Chrome is recommended). The USB cable is essential for connecting the board to the computer, indicated by the green LED lighting up, confirming a successful connection.

## Steps to Get Started with Arduino Mega

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

### DC Motor

- DC motors allow the robot to move forward and backward, powered by direct current.
### Servo

- Servos provide precise control of angular position and are used to move the wheels and camera.
### L298N Motor Driver

- The L298N driver controls the direction and speed of two DC motors using H-Bridge and PWM techniques.
### Pixy Camera

-The Pixy camera is a complete vision system that detects colors and lines, essential for navigation.

### Laser Cutter Machine

- We used a laser cutter to create precise parts, such as engine gears.

### Ultrasonic Sensor (HC-SR04)

-We utilized ultrasonic sensors to help the robot avoid obstacles and maintain a safe distance.
### Batteries

- We used four batteries to provide a total of 12 volts.
  

### Switches

- The robot includes two switches: one to power it on and off, and another to start the game.
For any further details or inquiries, feel free to reach out!

# (Time has betrayed us, but we will succeed in the end, God willing.)

------------------------------------------------------------------------------------
# 💻 رحلتنا فالبرمجة وخبراتنا


# Our Journey as a Programmer 💻

As a passionate programmer, I believe that the following skills and experiences define my path in the tech industry:

## Technical Skills
- **Proficient in Programming Languages**: 
  - Python 
  - Java 
  - JavaScript
  - Strong focus on developing efficient algorithms.
  - Arduino
  
- **Framework Knowledge**: 
  - Familiar with popular frameworks such as:
    - React for front-end development 
    - Django for back-end applications.

- **Web Development**: 
  - Skilled in HTML and CSS, enabling me to create responsive and user-friendly web applications.

## Soft Skills
- **Effective Communication**: 
  - Ability to convey technical concepts clearly and collaborate effectively with team members.
  
- **Problem-Solving**: 
  - Strong analytical skills that allow me to tackle complex challenges and devise innovative solutions.
  
- **Time Management**: 
  - Proficient in prioritizing tasks to meet deadlines in a fast-paced environment.

## Tools Knowledge
- **Version Control**: 
  - Experienced with Git and GitHub for managing code repositories and collaborating on projects.
  
- **Development Environments**: 
  - Comfortable using tools like Visual Studio Code and IntelliJ IDEA for efficient coding.
  
- **Continuous Integration**: 
  - Familiar with CI/CD tools like Jenkins and CircleCI to streamline the development process.

## Practical Experience
- **Open-Source Contributions**: 
  - Actively contribute to open-source projects, enhancing my coding skills and collaborating with developers worldwide.
  
- **Internships**: 
  - Completed internships at reputable companies, gaining hands-on experience in software development and team dynamics.

## Future Trends
- **AI and Machine Learning**: 
  - Currently exploring the fundamentals of artificial intelligence and its applications in software development.
  
- **Big Data Analytics**: 
  - Understanding how to analyze large datasets and extract meaningful insights is a key area of interest.

## Continuous Learning
- **Online Courses**: 
  - Enrolled in various online courses to stay updated on the latest technologies and programming practices.
  
- **Reading**: 
  - Regularly read books and articles on software development, design patterns, and emerging technologies.

## Community Engagement
- **Tech Conferences**: 
  - Attend tech meetups and conferences to network with professionals and learn from industry leaders.
  
- **Programming Communities**: 
  - Actively participate in online forums and communities to share knowledge and collaborate on projects.
