# Flowchart

<img width="830" alt="image" src="https://github.com/malakalhanafi02/robotmovement/assets/122760944/bedc091d-ded9-49a0-9512-5c3ca20158bc">


## Explanation

1. **Initialize Servo Positions**

2. **Move Right Leg Forward**:
   - **Right Hip (Servo 4)**: Move to 45 degrees.
   - **Right Knee (Servo 5)**: Move to 90 degrees.
   - **Right Ankle (Servo 6)**: Move to 45 degrees.
   - **Delay**: 500 ms.

3. **Move Left Leg Forward**:
   - **Left Hip (Servo 1)**: Move to 45 degrees.
   - **Left Knee (Servo 2)**: Move to 90 degrees.
   - **Left Ankle (Servo 3)**: Move to 45 degrees.
   - **Delay**: 500 ms.

4. **Move Right Leg Back**:
   - **Right Hip (Servo 4)**: Move to 90 degrees.
   - **Right Knee (Servo 5)**: Move to 180 degrees.
   - **Right Ankle (Servo 6)**: Move to 90 degrees.
   - **Delay**: 500 ms.

5. **Move Left Leg Back**:
   - **Left Hip (Servo 1)**: Move to 90 degrees.
   - **Left Knee (Servo 2)**: Move to 180 degrees.
   - **Left Ankle (Servo 3)**: Move to 90 degrees.
   - **Delay**: 500 ms.

6. **Repeat the Cycle**:
   - The loop continuously alternates between the right and left leg positions to simulate a walking motion.

### Human Movement Inspiration

The movement pattern for this robot mimics basic human walking steps:

- **Swing Phase**: One leg (right or left) is moved forward while the other leg remains in a fixed position.
- **Stance Phase**: After the swing phase, the leg moves to a back position, and the opposite leg is swung forward.

  
![image](https://github.com/malakalhanafi02/robotmovement/assets/122760944/ed3ae524-ca07-4f1c-a9ca-2e845f4d1f3c)



