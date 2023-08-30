# line_follower_bot

Line Follower Robot (LFR) is a simple autonomously guided robot that follows a line drawn on the ground to either detect a dark line on a white surface or a white line on a dark. The LFR is quite an interesting project to work on and learn the use of motors and arduino, that is why I started working on it. We will build a black line follower robot using Arduino Uno and some easily accessible components.

##Working of a Line Follower Robot

As stated earlier, line follower robot (LFR) follows a line, and in order to follow a line, robot must detect the line first. Now the question is how to implement the line sensing mechanism in a LFR. We all know that the reflection of light on the white surface is maximum and minimum on the black surface because the black surface absorbs maximum amount of light. So, we are going to use this property of light to detect the line. To detect light, either LDR (light-dependent resistor) or an IR sensor can be used. For this project, we are going with the IR sensor because of its higher accuracy. To detect the line, we place two IR sensors one on the left and other on the right side of the robot as marked in the diagram below. We then place the robot on the line such that the line lies in the middle of both sensors. We have covered a detailed Arduino IR sensor tutorial which you can check to learn more about the working of IR sensors with Arduino Uno.

Infrared sensors consist of two elements, a transmitter and a receiver. The transmitter is basically an IR LED, which produces the signal and the IR receiver is a photodiode, which senses the signal produced by the transmitter. The IR sensors emits the infrared light on an object, the light hitting the black part gets absorbed thus giving a low output but the light hitting the white part reflects back to the transmitter which is then detected by the infrared receiver, thereby giving an analog output. Using the stated principle, we control the movement of the robot by driving the wheels attached to the motors, the motors are controlled by a microcontroller.

##Components Required for Making Arduino Line Follower Robot

    1. Arduino Uno - 1Nos
    2. L293D motor driver- 1Nos
    3. IR sensor module -2 Nos
    4. 7.4 or 9V battery -1 Nos
    5. BO motor - 2 Nos
    6. Motor wheel - 2 Nos
    7. Castor wheel - 1 Nos
    8. Hobby robot chassis - 1 Nos
    9. Wires
    10. Screw


Line follower bot on display at STEX-22 , Competition organized by Institute of Radio Physics and Electronics, University of Calcutta.
<img src="https://user-images.githubusercontent.com/76748505/194532682-078ccc6a-8b73-4dcb-8e10-b11cbfd06ba3.JPG" alt="Garbage_Classifying_Bot" width="400"/>

Me (Second from Left) demonstrating the bot at STEX'22, annual technology Exhibit at my University.
<img src="https://user-images.githubusercontent.com/76748505/194536346-63116d81-4446-4606-a2a1-fb636123d5cd.jpg" alt="Demonstration_of_Bot" width="600"/>
