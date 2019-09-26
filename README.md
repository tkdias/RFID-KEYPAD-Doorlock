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




