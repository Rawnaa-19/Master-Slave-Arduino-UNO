# Master Slave Arduino UNO
## Table of Contents : 
1. [Introduction](#Introduction)
1. [A Master and a Slave](#A-Master-and-a-Slave)
    - [Circuit Components](#Master/Slave-Circuit-Components)
    - [Circuit Wiring](#Master/Slave-Circuit-Wiring)
    - [Arduino Code](#UArduino-Code)
    - [Code simulation](#Code-simulation)
1. [References](#References)
## Introduction
The second task for the Internet of Things Department is connecting two Arduino UNOs. To accomplish this task, I used the I2C protocol to make the Arduinos communicate with each other. The I2C "Inter-integrated circuit" is a serial communication protocol designed to send data along a single wire.(Campbell, 2021) The I2C protocol requires two connections: The first connection is used to send the data "SDA" and an additional connection for the clock signal "SCL" since it is a synchronous communication.(Campbell, 2021) 
To implement this protocol in this task, one Arduino will be the master, and the other Arduino will be the slave. Communication is initiated by the master Arduino, which generates the clock signal.(Master Reader/Slave Sender, n.d.)The slave Arduino has its own unique address, so it is easy to identify it.(Master Reader/Slave Sender, n.d.)<br><br> 
<kbd> **Figure 1** <br><br>*I2C Connections*<br><br> <kbd>![image](https://github.com/Rawnaa-19/Master-Slave-Arduino-UNO/assets/106926557/f9fc7f67-7fa0-4b80-a5d7-9328e8db86d3)(Understanding the Differences Between UART and I2C, 2023)</kbd></kbd>

## A Master and a Slave
The goal of this task is to control an LED with a push button, where the push button is connected to the master Arduino and the LED is connected to the slave Arduino.

### Master/Slave Circuit Components
1. Two Arduino UNOs
2. Push button
3. LED
4. 220 ohm resistor
5. Breadboard
6. Wires

### Master/Slave Circuit Wiring
As mentioned before, the I2C protocol requires two connections "SDA" and "SCL". The SDA line corresponds to pin A4 and the SCL line corresponds to pin A5 on the Arduino UNO. In order to establish communication, connect these pins A4 and A5 to the same pins on the other Arduino. Connect the two Arduinos together via their GND pins.
The push button is connected to pin 7 of the Master Arduino. And the LED is connected to pin 13 of the slave Arduino.<br><br> 
<kbd> **Figure 2** <br><br>*Master/Slave Circuit Wiring*<br><br> <kbd>![image](https://github.com/Rawnaa-19/Master-Slave-Arduino-UNO/assets/106926557/72c9089a-36ea-422f-87e2-b930204cf04a)</kbd></kbd>
