# Arduino Electronic Safe

This project implements an electronic safe powered by an Arduino Uno. It's a perfect blend of hardware and software that provides a secure way to store your valuables.

## Features

- **User Interface**: The safe uses a [16x02 LCD Monitor](https://wokwi.com/playground/lcd1602) and a [Membrane Keypad](https://wokwi.com/playground/keypad) for user interaction. The LCD displays the status of the safe and instructions for the user, while the keypad is used for inputting the password.

- **Lock Mechanism**: The lock mechanism is powered by a Servo motor. When the correct password is entered, the Servo motor turns to unlock the safe.

- **Persistent Storage**: The state of the safe (locked/unlocked), as well as the secret code, are stored in the Arduino's [EEPROM](https://wokwi.com/playground/eeprom). This ensures that the code isn't wiped even when the power goes off.

- **Password Suggestion**: The safe suggests a random password to the user at the password prompt. This feature helps users set strong and random passwords for their safe.
  
- **Password Strength Indicator**: After setting the password, the safe provides a password strength indicator to help users assess the strength of their chosen password. This feature helps users create stronger and more secure passwords.

## Authors

This project was created by:

- Shobhit (2021UCS1618)
- Prachi Sah (2021UCS1702)
- Ujjawal (2021UCS1659)