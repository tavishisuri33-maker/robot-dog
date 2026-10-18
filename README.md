# robot-dog
Project Summary: The goal is to create a robot dog with hip and knee of each leg using servo,ESP32 and MPU6050 using Wokwi.
The main aim of this project is to help the dog walk, crouch, tall and stop according to the user input.

Wokwi link:

Working: The project using the connections of the mentioned hardware devices with a suitable non delaying code.
Each leg has two servo, one for hip and one for knee.The hip helps move forward and backward and knee is used for bending.
The front left hip leg is connected to pin 13 of the ESP and with its knee connected to 12.
The front right hip leg is connected to pin 14 of the ESP and with its knee connected to 27.
The back left hip leg is connected to pin 26 of the ESP and with its knee connected to 25.
The back right hip leg is connected to pin 33 of the ESP and with its knee connected to 32.
The above connections are done using green color wire, whereas the brown wire is connected to gnd and red wire to 5V.
The MPU6050 green wires (SDA and SCL) is connected to pin 21 and 22 of ESP.
The MPU6050 red wire connected to 3V (operates on 3.3V) and black wire to gnd of ESP.

Power Budget:
We are given 12 servos which are rated at 6V.
Normal current: Assuming that each servo requires 0.5A current to move the robodog.
12 * 0.5= 6A
Power at normal current: 6 * 6= 36W
Peak current: Assuming that each servo at peak is rated 1A.
12 * 1=12A
power at peak: 12 * 6= 72W
For such requirements 2S LiPo battery is better since it would draw more power. Rounding off the power at peak to 80W, the battery can supply 7.4V which is more than the rated 6V which supplies around 100W of power which is more than what is required.
The capacity of the battery can be from 2200khw - 5000khw depending on the power.



