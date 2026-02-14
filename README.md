# IR Remote Motor Control (TX + RX)

This project uses an Arduino and an IR remote system to control a motor wirelessly.

## 📌 Project Overview
The system consists of:
- IR Transmitter (TX)-arduino uno, mosfet, ir led, 1k;1M;140ohm resistors, POT and 2 buttons 
![TX circuit diagram](https://github.com/user-attachments/assets/fe9a07ec-5c85-49eb-bf73-a1b1309ef237)
<img width="810" height="1080" alt="image" src="https://github.com/user-attachments/assets/21e7e831-1e75-4e2b-b094-96320907b557" />


- IR Receiver (RX)-arduino uno, irm3638t(ir receiver), 5x1k resistors, green led, dc motor, 4x2n2222 transistors
![RX circuit diagram](https://github.com/user-attachments/assets/6acb8795-e01d-4ebb-a62b-1d8a32f165dd)
<img width="810" height="1080" alt="image" src="https://github.com/user-attachments/assets/9ce6dcef-3cd9-4e06-801d-61dca1c09495" />  


The transmitter sends constantly IR signals, but when a button is pressed it sends a different signal 
The receiver decodes the signal and controls the motor accordingly.

## 🧠 What This Project Demonstrates
- IR signal transmission and decoding
- Use of the IRremote library
- Digital signal processing
- Motor control logic
- Embedded C++ programming

## 📂 Files Included
- `TX_IR_kontrolaMotora.ino` – IR transmitter code
- `RX_IR_kontrolaMotora.ino` – IR receiver and motor control code

## 🚀 How It Works
The tx send constantly ir signals, but when no button is pressed, the signal is off; off. But when B1 is pressed-signal is on; off(you get the idea)
And the POT controls the PWM on the RX output pins.
So when tx button 1 is pressed-rx pin9 is on. And when button 2 is pressed-rx pin5 is on.
The tx send constantly beacuse it sets the PWM, and the buttons give instructions to turn on the pins

Created as part of Hack Club Blueprint.

videos:
https://github.com/user-attachments/assets/b371348b-3e40-450a-a603-be2d543e8e3a
https://github.com/user-attachments/assets/998ba6f6-3401-430d-885f-fe101a74188d
https://github.com/user-attachments/assets/7f66e379-3ef2-4de0-b5f1-2564e668604d
https://github.com/user-attachments/assets/f0c71a79-ffcb-4000-9000-4d54b1c272e9



