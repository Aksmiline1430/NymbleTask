# NymbleTask
Firmware (Arduino) Documentation:
Overview:
This firmware facilitates bidirectional communication between a PC and an MCU (Arduino) via UART. It receives text data from the PC, stores it in EEPROM, and then retrieves and transmits the data back to the PC.

Setup and Requirements:
Hardware:
Arduino Uno (or any compatible MCU)
Software:
Arduino IDE
Implementation Steps:
Setup UART Communication: Initialize serial communication with the specified baud rate.
Receive Data from PC: Continuously check for incoming data from the PC via UART.
Store Data in EEPROM: As data is received, store it in the EEPROM memory byte by byte.
Transmit Data back to PC: After receiving all data, retrieve it from EEPROM and transmit it back to the PC.
Reset EEPROM Address: Once data transmission is complete, reset the EEPROM address for future use.
Code Comments:
Each function and critical section of the code is accompanied by descriptive comments to explain its purpose and functionality.
Configuration Parameters:
Baud rate: 2400
Testing:
The firmware has been tested with various text inputs to ensure correct reception, storage, retrieval, and transmission of data.
Java (PC) Code Documentation:
Overview:
This Java program facilitates communication with the MCU (Arduino) by transmitting text data to it via serial communication and receiving the transmitted data back from the MCU.

Setup and Requirements:
Java Development Kit (JDK)
RXTX library for serial communication in Java
Implementation Steps:
Initialize Serial Port: Connect to the specified serial port and configure parameters such as baud rate, data bits, and stop bits.
Transmit Data to MCU: Send the text data byte by byte to the MCU via serial communication.
Receive Data from MCU: Continuously read incoming data from the MCU until all expected data is received.
Display Received Data: Print the received data on the console screen of the PC.
Code Comments:
The Java code includes comments to explain each step of the communication process and clarify the functionality of each section.
Testing:
The Java program has been tested with various text inputs to ensure correct transmission and reception of data between the PC and MCU.
