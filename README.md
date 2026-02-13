## 📌 Project Overview
The system consists of:
- IR Transmitter (TX)-arduino uno, mosfet, ir led, 1k;1M;140ohm resistors, POT and 2 buttons 
![TX circuit diagram](https://github.com/user-attachments/assets/fe9a07ec-5c85-49eb-bf73-a1b1309ef237)
<img width="810" height="1080" alt="image" src="https://github.com/user-attachments/assets/21e7e831-1e75-4e2b-b094-96320907b557" />


- IR Receiver (RX)-arduino uno, irm3638t(ir receiver), 5x1k resistors, green led, dc motor, 4x2n2222 transistors
![RX circuit diagram](https://github.com/user-attachments/assets/6acb8795-e01d-4ebb-a62b-1d8a32f165dd)
<img width="810" height="1080" alt="image" src="https://github.com/user-attachments/assets/9ce6dcef-3cd9-4e06-801d-61dca1c09495" />  


The transmitter sends constantly IR signals, but when a button is pressed it sends a different signal 
@@ -30,3 +35,5 @@ So when tx button 1 is pressed-rx pin9 is on. And when button 2 is pressed-rx pi
The tx send constantly beacuse it sets the PWM, and the buttons give instructions to turn on the pins

Created as part of Hack Club Blueprint.

videos:

