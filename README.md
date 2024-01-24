# Electronic Safe with Face Authentication

This project combines an Arduino-based electronic safe with a Python-based face authentication system. The electronic safe is controlled by an Arduino Uno and provides a secure way to store your valuables. The face authentication system uses OpenCV and DeepFace to verify the identity of the user.

## Electronic Safe

The electronic safe is implemented in C++ for the Arduino platform. It uses a 16x02 LCD Monitor and a Membrane Keypad for user interaction. The lock mechanism is powered by a Servo motor. When the correct password is entered, the Servo motor turns to unlock the safe. The state of the safe (locked/unlocked), as well as the secret code, are stored in the Arduino's EEPROM. This ensures that the code isn't wiped even when the power goes off.

The electronic safe code is located in the [`electronic-safe`](command:_github.copilot.openRelativePath?%5B%22electronic-safe%22%5D "electronic-safe") directory. The main file is [`electronic-safe.ino`](command:_github.copilot.openSymbolInFile?%5B%22electronic-safe%2Felectronic-safe.ino%22%2C%22electronic-safe.ino%22%5D "electronic-safe/electronic-safe.ino"), and the `SafeState` class, which manages the state of the safe, is defined in [`SafeState.cpp`](command:_github.copilot.openSymbolInFile?%5B%22electronic-safe%2FSafeState.cpp%22%2C%22SafeState.cpp%22%5D "electronic-safe/SafeState.cpp") and [`SafeState.h`](command:_github.copilot.openSymbolInFile?%5B%22electronic-safe%2FSafeState.h%22%2C%22SafeState.h%22%5D "electronic-safe/SafeState.h").

## Face Authentication

The face authentication system is implemented in Python. It uses OpenCV to capture video from the webcam and DeepFace to verify the identity of the user. If the user's face matches a reference image, the system opens a web browser and navigates to a specified URL.

The face authentication code is located in the [`faceAuthentication`](command:_github.copilot.openRelativePath?%5B%22faceAuthentication%22%5D "faceAuthentication") directory. The main file is [`main.py`](command:_github.copilot.openSymbolInFile?%5B%22faceAuthentication%2Fmain.py%22%2C%22main.py%22%5D "faceAuthentication/main.py").

## Authors

This project was created by:
- Shobhit (2021UCS1618)
- Prachi Sah (2021UCS1702)
- Ujjawal (2021UCS1659)

## How to Run

To run the electronic safe, upload the [`electronic-safe.ino`](command:_github.copilot.openRelativePath?%5B%22electronic-safe%2Felectronic-safe.ino%22%5D "electronic-safe/electronic-safe.ino") file to your Arduino Uno.

To run the face authentication system, you need to have Python, OpenCV, DeepFace, and Selenium installed. You can then run the [`main.py`](command:_github.copilot.openRelativePath?%5B%22faceAuthentication%2Fmain.py%22%5D "faceAuthentication/main.py") file.

Please note that you need to adjust the paths to the reference images in the [`main.py`](command:_github.copilot.openRelativePath?%5B%22faceAuthentication%2Fmain.py%22%5D "faceAuthentication/main.py") file to match your setup.