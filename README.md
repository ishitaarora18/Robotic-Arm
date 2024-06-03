# Robotic-Arm

Robotic Arm - The Soul of Industrial Automation

Problem Statement : A number of situations exist where it is not possible for a human operator to do an activity:- due to a level of danger or difficulty involved. They may involve-
1. Taking readings from an active volcano
2. Entering a building on fire
3. Diffusing a bomb
4. Collecting a radioactive sample
Robotic systems are far superior in ensuring the accuracy of the system under adverse circumstances wherein a human operator may lose his/her composure and focus. So, we built a robotic arm controlled by Arduino.

Installing libraries:
1. Download the library from http://bit.ly/motorShieldLibrary
2. Uncompress the ZIP file onto your desktop
3. Rename the uncompressed folder AFMotor
4. Place the AFMotor folder into your arduinosketchfolder/libraries folder. For Windows, this will probably be something like MY Documents/Arduino/libraries for Mac it will be something like Documents/arduino/libraries. If this is the first time you are installing a library, you'll need to create the libraries folder. Make sure to call it libraries exactly, no caps, no other name.
5. Quit and restart the Arduino. You should now have a submenu called File->Examples->AFMotor->MotorParty
6. If not, Check that inside the libraries folder there is the AFMotor folder, and inside AFMotor isAFMotor.cpp AFMotor.h and some other files

Using DC Motors:
1. To connect a motor, simply solder two wires to the terminals and then connect them to either the M1, M2, M3, or M4
2. Make sure you include library
#include <AFMotor.h>
3. Create the AF_DCMotor object with AF_DCMotor(motor#)
Motor# tells motor is connected to which port, 1, 2, 3 or 4
4. Then you can set the speed of the motor using setSpeed(speed) where the speed ranges from 0 (stopped) to 255 (full speed)
5. To run the motor, call run(direction) where direction is FORWARD, BACKWARD or RELEASE.
   RELEASE – Stops motor
   FORWARD/BACKWARD – Runs motor clockwise/anticlockwise (it depends how you connect motor to battery)

Using Arduino IDE:
1. Each Arduino file is called sketch 
2. When you open Arduino IDE, you would see 2 functions written in sketch
   setup()
   loop()
   
setup()
	The setup() function is called when a sketch starts. It is used to initialize variables, pin modes, start using libraries, etc. This function will only run once, after each powerup or reset of the Arduino 
  board.
  

loop()
	The loop() function does precisely what its name suggests, and loops consecutively, allowing the program to change and respond. It is used to actively control the Arduino board. 





