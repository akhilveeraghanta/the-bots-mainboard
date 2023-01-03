# The Bots Mainboard

The majoriy of this board/schematics were created watching [Phils Lab](https://www.youtube.com/@PhilsLab) on youtube 

The soccer playing AI will compute target velocities for all 6 robots and send them over USB to the mainboard, which will then pack the velocity data into a radio payload and send it over. Each robot will have a mainboard, receive the pacet over radio and put the velocity command onto the CAN Bus as a new setpoint for the motor drivers. 

![](docs/bots.drawio.png)

So the main goal of the board is to act as a radio to CAN bridge if flashed as a robot, and a radio to USB bridge if flashed as a dongle and plugged into the computer running AI.

![BoardyMcBoardFace](https://user-images.githubusercontent.com/31548846/210305385-8d1ab096-a10a-4936-882e-6e1a36c88515.png)

Additionally, the ball detector circuit, when plugged into a robot will be facing the "mouth" of the robot to detect any balls that enter.

Here is one of our competitors, UBC Thunderbots's robot to put this board into perspective. (We don't have robots yet)

![image](https://user-images.githubusercontent.com/31548846/210306025-341cc2d2-a319-49ce-87f6-c7ef307469b7.png)

and more info about robocup can be [found here](https://ssl.robocup.org/)
