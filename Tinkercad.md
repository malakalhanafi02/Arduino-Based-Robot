# TINKERCAD

## [Link to Tinkercad project](https://www.tinkercad.com/things/dQ80jAch3RA-terrific-bruticus-kasi/editel?sharecode=Q9g24-NYfmY0KyevuSnWGsaTHZ9LJBCwp-XEFY9Cbm8)

  <img width="997" alt="image" src="https://github.com/malakalhanafi02/robotmovement/assets/122760944/5f46b999-f36d-4eb7-804c-722e96bfc5d3">

### Components

- 1 x Arduino Uno
- 6 x Servo Motors
- 1 x Breadboard
- Jumper Wires
- 1 x External Power Supply (5V 6A)

### Wiring

1. **Servo Connections**:
   - **Signal Wires**:
     - Servo 1 (Right Hip): Connect to Arduino digital pin 3
     - Servo 2 (Right Knee): Connect to Arduino digital pin 5
     - Servo 3 (Right Ankle): Connect to Arduino digital pin 6
     - Servo 4 (Left Hip): Connect to Arduino digital pin 9
     - Servo 5 (Left Knee): Connect to Arduino digital pin 10
     - Servo 6 (Left Ankle): Connect to Arduino digital pin 11

   - **Power and Ground**:
     - All servo power (Red) wires are connected to the positive rail on the breadboard.
     - All servo ground (Black/Brown) wires are connected to the ground rail on the breadboard.

2. **External Power Supply**:
   - **Positive Terminal (5V)**: Connect to the positive rail on the breadboard.
   - **Ground Terminal**: Connect to the ground rail on the breadboard.

3. **Arduino Connections**:
   - Connect the Arduino's GND to the ground rail on the breadboard to ensure a common ground.
   - The Arduino is powered through the USB connection to the computer.

### Code

```cpp
#include <Servo.h>

Servo servo1; // Right hip
Servo servo2; // Right knee
Servo servo3; // Right ankle
Servo servo4; // Left hip
Servo servo5; // Left knee
Servo servo6; // Left ankle

void setup() {
  servo1.attach(3);
  servo2.attach(5);
  servo3.attach(6);
  servo4.attach(9);
  servo5.attach(10);
  servo6.attach(11);
}

void loop() {
  servo1.write(45);  
  servo2.write(90);    
  servo3.write(45);    
  delay(500);            

  servo4.write(45);  
  servo5.write(90);    
  servo6.write(45);    
  delay(500);             

  servo1.write(90);  
  servo2.write(180);   
  servo3.write(90);    
  delay(500);            

  servo4.write(90);  
  servo5.write(180);   
  servo6.write(90);    
  delay(500);  
}
```
 ---

### Why Use an External Power Supply?

Multiple servo motors can draw significant amounts of current and the Arduino's power supply is not enough to provide the necessary current for all six servos. 

- Using an external **5V 6A** power supply ensures that each servo receives enough power, preventing potential issues such as voltage drops and overloading the Arduino.
