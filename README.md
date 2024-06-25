Arduino - Caesar Cipher (Encryption/Decryption)

This project is an Arduino-based Caesar cipher encryption and decryption system using a LiquidCrystal display and serial communication. 
The system allows users to input a word and either encrypt or decrypt it using a shift value of 3.

Hardware Requirements:
- Arduino board (e.g., Arduino Uno)
- 16x2 LiquidCrystal Display (LCD)
- Jumper wires
- Breadboard
  
Software Requirements:
- Arduino IDE
- LiquidCrystal library (included by default in the Arduino IDE)

Circuit Diagram
Connect the LCD to the Arduino as follows:

![image](https://github.com/Maksymus333333/arduino_cipher/assets/134223557/45870845-8073-4dfc-ad0e-10be4761e628)

Installation and Setup

1. Connect the hardware:

- Set up the circuit as described in the circuit diagram.

2. Upload the Code:

- Open the Arduino IDE.
- Copy the provided code into a new sketch.
- Connect your Arduino board to the computer.
- Select the correct board and port from the Tools menu.
- Upload the sketch to the Arduino board.

Code Overview

The code initializes the LCD and sets up serial communication.

It waits for user input via the Serial Monitor to either encrypt 

or decrypt a given word using a Caesar cipher with a shift value of 3. 

The results are displayed on both the Serial Monitor and the LCD.



  Main Components

1. Initialization:

- Initializes the LCD with 16 columns and 2 rows.
- Displays "Szyfrowanie!" (Encryption!) on the LCD.


2. User Interaction:

- Prompts the user to enter 'e' for encryption or 'd' for decryption followed by the word.
- Reads the user input from the Serial Monitor.
- Clears the LCD and displays the results of the encryption or decryption.


3. Encryption and Decryption Functions:

- encrypt(String text, int s): Encrypts the input text using a Caesar cipher.
- decrypt(String text, int s): Decrypts the input text by reversing the encryption process.

Usage

1. Open the Serial Monitor:

- After uploading the sketch, open the Serial Monitor in the Arduino IDE.

2. Enter Command:

- Type 'e' followed by a word to encrypt or 'd' followed by a word to decrypt (e.g., e hello or d khoor).

3. View Results:

- The original and processed words will be displayed on the Serial Monitor and the LCD.


Example

  - Input e hello:
    - Output on Serial Monitor

     ![image](https://github.com/Maksymus333333/arduino_cipher/assets/134223557/eff76db6-cd00-41f2-a3d1-2410c449bc83)

    - Output on LCD
    
     ![image](https://github.com/Maksymus333333/arduino_cipher/assets/134223557/51b0dfec-1cd3-44ef-9ff0-8bdab5117121)

  - Input d khoor:
    - Output on Serial Monitor
    
    ![image](https://github.com/Maksymus333333/arduino_cipher/assets/134223557/ed7913f5-2c23-4009-ac8f-ccf7009b2b6f)

    - Output on LCD

    ![image](https://github.com/Maksymus333333/arduino_cipher/assets/134223557/027bc009-684c-407a-bea2-3ac911391aef)


Troubleshooting

- Ensure all connections are correct and secure.
- Verify the contrast of the LCD using the potentiometer.
- Check that the correct board and port are selected in the Arduino IDE.
- Make sure the baud rate in the Serial Monitor is set to 9600.

License

  This project is open-source and can be freely used and modified. Contributions and improvements are welcome.

  Don't forget to put an asterisk :)

Author
Developed by Maksymus333333



       

