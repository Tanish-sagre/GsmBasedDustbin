Smart Dustbin System
This Arduino sketch is designed to create a Smart Dustbin system using an Arduino board, a servo motor, a PIR motion sensor, and an ultrasonic sensor. The system incorporates GSM communication to send a notification when the dustbin is full.

Components Used:
Arduino board
Servo motor
PIR motion sensor
Ultrasonic sensor
GSM module (SoftwareSerial library is used for communication)
LEDs (indicating different levels of trash in the dustbin)

Pin Configuration:
trigpin1 (Ultrasonic sensor trigger pin): 12
echopin1 (Ultrasonic sensor echo pin): 13
led1, led2, led3, led4 (LEDs indicating trash levels): 5, 6, 7, 8
pirPin (PIR motion sensor pin): 4
Servo motor control pin: 9
GSM module pins (Rx, Tx): 2, 3

Functionality:
The system uses a PIR motion sensor to detect if someone is near the dustbin. When motion is detected, it opens the lid using a servo motor.
The ultrasonic sensor is used to measure the level of trash in the dustbin. Different LED indicators light up based on the trash level.
If the trash level reaches a critical point (close to full), a message is sent using the GSM module to a specified phone number.
The system closes the lid after a delay if no motion is detected.

Usage:
Ensure all the components are connected as per the specified pin configuration.
Upload the provided Arduino sketch to your Arduino board.
Power up the system and monitor the serial monitor for debug information.
Important Notes:

The GSM module is used to send an SMS when the dustbin is full. Make sure to configure the GSM module with the correct mobile number (+919589223284 in this example).
Adjust the distance conditions in the ultrasonic sensor section based on your dustbin's physical dimensions.
Feel free to customize and enhance the code according to your requirements.
