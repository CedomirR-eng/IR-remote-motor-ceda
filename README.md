# IR Remote Motor Control (TX + RX)

This project uses an Arduino and an IR remote system to control a motor wirelessly.

## 📌 Project Overview
The system consists of:
- IR Transmitter (TX)-arduino uno, mosfet, ir led, 1k;1M;140ohm resistors, POT and 2 buttons 

- IR Receiver (RX)-arduino uno, irm3638t(ir receiver), 5x1k resistors, green led, dc motor, 4x2n2222 transistors


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
