# Bluetooth Controlled Smart Car
>## Overview.
>>This project represents Bluetooth controlled robotic car. The project aims in designing a Robot that can be operated using Android mobile phone. The controlling of the Robot is done wirelessly through Android smart phone using the Bluetooth feature present in it. We present a review of robots controlled by mobile phone via moving the robot upward, backward, left and right side by android application. Here in the project the Android smart phone is used as a remote control for operating the Robot. The controlling device of the whole system is a Microcontroller. Bluetooth module, DC motors are interfaced to the Microcontroller.<br/>
> ## Concept Behind the Project.
>>When using the MOSFET as a switch we can drive the MOSFET to turn “ON” faster or slower, or pass high or low currents. This ability to turn the power MOSFET “ON” and “OFF” allows the device to be used as a very efficient switch with switching speeds much faster than standard bipolar junction transistors. In this project MOSFET is used as switch to control the motors.
> ## Software Required.
>>* Proteus Design Suite<br/>
>>* Arduino IDE <br/>
> ## Hardware Required.
>> * Arduino UNO<br/>
>> * Bluetooth Module (HC-06)<br/>
>> * Arduino USB<br/>
>> * MOSFET Transistor<br/>
>> * Servo Motor<br/>
>> * 9V DC Motor<br/> 

> ## Circuit Diagram:
>>

> ## Working
>> * First connect the power and ground of the Arduino to the power and ground on the left side of your breadboard.<br/>
>> * Next connect the first battery snaps power and ground to the right side of the breadboard. Connect the other Battery snaps power to the Vin pin on the Arduino, and the ground on the battery snap to ground on the Arduino.<br/>
>> * Connect the servo motor's power pin to the 5V on the left side of the breadboard, the ground pin to ground on the left side of the breadboard, and the center pin of the servo motor to pin 9 on the Arduino. The center pin is the one that will allow us to control the angle that the servo is set at.<br/>
>>  * Connect VCC pin of the HC-06 Bluetooth Module to 5V on the left side of the breadboard, and the GND pin to the ground on the left side of the breadboard. Refrain from plugging in the TX and RX pins until you upload the program onto the Arduino board, because the board will not accept the program while those pins are plugged in. After you have uploaded the program to the Arduino plug the TX pin of the HC-06 into the RX pin of the Arduino, and the RX pin of the HC-06 into the TX of the Arduino.<br/>
>>  * Next in line is the motor. Because the Arduino only produces a maximum of 5V it is not enough to propel the card forward, however we still need to be able to control the motor using the Arduino. We will do this using a component called a MOSFET transistor. The MOSFET has 3 pins, a gate, a source, and a drain. when we apply 5V to the gate, power will be able to flow through from the drain to the source. With this in mind we will connect the gate pin of the MOSFET to pin 6 of the Arduino. This will allow us to link the other 2 pins of the MOSFET together by putting power out of pin 10. Next connect the source of the MOSFET to ground on the right side of the breadboard. Then connect one end of the motor to the drain pin on the MOSFET. <br/>
>>  * Connect a diode from the drain pin to the power bar on the right side of the breadboard. This diode in parallel will stop something called back-voltage. When a motor spins around it creates electricity like a generator, and this electricity can flow in the opposite direction that the circuit is running. This can cause problems, and in order to stop the electricity from doing this we need to insert a diode in parallel with the motor. Now connect the other end of the motor to the power bar on the right side of the breadboard.<br/>
>>  * We need to put the program code on the Arduino Uno in order to control the car, Download and open it in the Arduino IDE. We will upload this to the Arduino board in order to control the car.<br/>
>>  * Finally all you need is a freely spinning axle with 2 back wheels, a front wheel that can be attached to the servo motor, and a platform above or in between that can house the circuit board and breadboard. The motor also needs to be able to be attached to the rear axle by an elastic band so that the back tires can spin. Basically you just attach the circuit board and breadboard together in a package, and attach it to the platform made. Hook up the motor to the axle with an elastic band and then your almost set.<br/>
>>  * You need an Android phone for this to work, and then you go into google play and find the app called "Smart Bluetooth". Connect this to the HC-06 Bluetooth Module and your good to go!<br/>


>> For live simulation [Click here](https://drive.google.com/file/d/1IdVjetmgshf5lBt1eXNezATNBO3fBiXf/view?usp=sharing) 
