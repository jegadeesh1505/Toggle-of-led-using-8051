# Toggle-of-led-using-8051

8051 Assembly Program to Toggle an LED Using Timer 0 Mode1 with 2ms Delay in port 2.0.

# Aim:
To write and simulate an Assembly Language Program using the 8051 microcontroller to Toggle an LED Using Timer 0 Mode1 with 2ms Delay in port 2.0.
# Software required:
* Keil µVision IDE
* 8051 Assembler (A51)

# Algorithm:

1. **Initialize Port and Timer Mode**
   * Clear P2.0 (LED OFF).
   * Set Timer 0 in Mode 1 (16-bit timer).

2. **Load Timer Registers**
   * Load TH0 = F7H and TL0 = CEH for 2 ms delay.

3. **Start Timer**
   * Clear TF0 flag and set TR0 to start Timer 0.

4. **Wait for Overflow**
   * Monitor TF0 flag; when it becomes 1, stop the timer and clear TF0.

5. **Toggle LED and Repeat**
   * Complement P2.0 to toggle LED.
   * Jump back to repeat the delay continuously.

# Program:




# Output From Keil:






# Manual Calculation:



# Result:
Thus, the 8051 Assembly Language Program to blink an LED with a 250 ms delay using Timer1 in Mode1 was successfully written, assembled, and simulated using Keil µVision.
The LED connected to Port 0.5 was observed to toggle every 250 ms.

  
