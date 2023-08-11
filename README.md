# Master Slave Arduino UNO
## Table of Contents : 
1. [Introduction](#Introduction)
1. [A Master and a Slave](#A-Master-and-a-Slave)
    - [Circuit Components](#Circuit-Components)
    - [Circuit Wiring](#Circuit-Wiring)
    - [Arduino Code](#UArduino-Code)
    - [Code simulation](#Code-simulation)
1. [References](#References)
## Introduction
The second task for the Internet of Things Department is connecting two Arduino UNOs. To accomplish this task, I have used the I2C protocol to make the Arduinos communicate with each other.The I2C "Inter integrated circuit" is a serial communication protocol used to send data along a signle wire.(Campbell, 2021)The I2C is  has two connections the first connection is used to send the data "SDA" and an additional connection for the clock signal "SCL" since it is a synchronys communication.(Campbell, 2021)  However, the I2C has another wire  Where one of them is the master and the other one is the slave.
