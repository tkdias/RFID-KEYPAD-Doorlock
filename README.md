# RFID-KEYPAD-Doorlock
In this post, you are going to learn about how to build an RFID and Keypad based door lock using Arduino. To open the door, the user will have to first scan the right tag and then he will have to enter the correct password. On scanning the wrong tag or on entering the wrong password, the system will deny access.

# Required Components for RFID and Keypad Based Door Lock using Arduino
The components you are going to require for RFID and Keypad Based Door Lock using Arduino are as follows

Arduino Uno or any other Arduino
I2C LCD
MFRC522 RFID Reader
Tags
SG90 Servo motor
4X4 Keypad or 4X3 Keypad
3 X LED’s (Red, Green, Blue)
3 X 220 ohm resistors
Buzzer
6 to 12V Power source (I have used 3 X 18650 cells)

# Circuit Diagram and Explanation

The RFID reader communicates with the Arduino through the SPI protocol and different Arduino boards have different SPI pins. I have described the connections of RFID Reader with different Arduino boards in the below table.

![alt text](https://github.com/tkdias/RFID-KEYPAD-Doorlock/blob/master/Image-0001.PNG)

To test if the RFID reader is working properly or not, upload the “dumpinfo” from the examples in the Arduino and see if it is showing the information of the tags on the serial monitor or not. If you are new to RFID, then follow this tutorial | RFID basics and RFID module interfacing with Arduino

The I2C LCD communicates with the Arduino through the I2C protocol. Different Arduino boards have different I2C pins. The I2C pins on Arduino Uno and Arduino Nano are A4, A5. The below table describes the connections of different Arduino’s with I2C LCD.

![alt text](https://github.com/tkdias/RFID-KEYPAD-Doorlock/blob/master/Image-0002.PNG)

Next we are going to connect the keypad with Arduino. The 4X4 keypad has 8 connections but we don’t require the last column of keypad. We only require numbers for the password. So we won’t use the last pin of keypad which is for fourth column. Connections for keypad with Arduino are given in below table. You can also use 4X3 keypad instead of 4X4 keypad.

![alt text](https://github.com/tkdias/RFID-KEYPAD-Doorlock/blob/master/Image-0003.PNG)

The below table describes the connections of Arduino with other components.

![alt text](https://github.com/tkdias/RFID-KEYPAD-Doorlock/blob/master/Image-0004.PNG)

In the end, connect the power source to the Arduino. I have used three 18650 cells. We can give 6 to 12V to the Arduino through the barrel jack.

![alt text](https://github.com/tkdias/RFID-KEYPAD-Doorlock/blob/master/Image-0005.PNG)

