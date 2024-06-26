# SMART-TRAFFIC-CONTROL
Density Based Traffic Signal System using Microcontroller
Nowadays, controlling the traffic becomes major issue because of rapid increase in automobiles and also because of large time delays between traffic lights. So, in order to rectify this problem, we will go for density based traffic lights system. This article explains you how to control the traffic based on density.

In this system, we will use IR sensors to measure the traffic density. We have to arrange one IR sensor for each road; these sensors always sense the traffic on that particular road. All these sensors are interfaced to the microcontroller. Based on these sensors, controller detects the traffic and controls the traffic system.

Density Based Traffic Signal System Circuit Principle:
The main heart of this traffic system is microcontroller. IR sensors are connected to the PORT C (PC0, PC1, PC2, and PC3) of the microcontroller and traffic lights are connected to PORT B and PORT D. If there is a traffic on road then that particular sensor output becomes logic 0 otherwise logic 1. By receiving these IR sensor outputs, we have to write the program to control the traffic system.

If you receive logic 0 from any of these sensors, we have to give the green signal to that particular path and give red signal to all other paths. Here continuously we have to monitor the IR sensors to check for the traffic.
Circuit Components
ATmega8 controller
PCB board
IR sensors -4
LED’s-12(4-red,4-green,4-yellow)
12v Battery or adaptor
Serial cable
Connecting wires

This circuit consists of 4 IR sensors, atmega8 microcontroller, 4 traffic lights.

IR transmitter looks like an LED. This IR transmitter always emits IR rays from it. The operating voltage of this IR transmitter is 2 to 3v. These IR (infra red) rays are invisible to the human eye. But we can view these IR rays through camera.

IR receiver receives IR rays that are transmitted by IR transmitter. Normally IR receiver has high resistance in order of mega ohms, when it is receiving IR rays the resistance is very low. The operating voltage of IR receiver also 2 to 3V.

We have to place these IR pair in such a way that when we place an obstacle in front of this IR pair, IR receiver should be able to receive the IR rays. When we give the power, the transmitted IR rays hit the object and reflect back to the IR receiver.

Instead of traffic lights, you can use LEDs (RED, GREEN, YELLOW). In normal traffic system, you have to glow the LEDs on time basis. If the traffic density is high on any particular path, then glows green LED of that particular path and glows the red LEDs for remaining paths.

In normal traffic system, we allow the traffic for a time delay of 1 minute for each path.

How to Operate Density based Traffic Signal System Circuit?
Connect 12V battery or adaptor to the development board.
Switch on the supply.
Burn the program to the ATmega8 microcontroller by keeping the programming switch sw2 in program mode.
Connect four IR sensors to PORT C.
Connect LEDs to PORT B and PORT D.
Arrange all this LED’s same as like traffic lights.
Arrange one IR sensor for each road.
Now you can see the normal traffic system based on time basis.
Now if you place any obstacle in front of any IR sensor, then the system allows the traffic of that particular path by glowing GREEN light.
Finally, turn off the board power supply.
Limitations of this Circuit:
IR sensors sometimes may absorb normal light also. As a result, traffic system works in improper way.
IR sensors work only for fewer distances.
We have to arrange IR sensors in accurate manner otherwise they may not detect the traffic density.


