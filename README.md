# Analog PID Controller using LTSpice

This project demonstrates the working of a PID (Proportional-Integral-Derivative) controller built using operational amplifiers in **LTSpice**. The simulation shows how each component of a PID controller — P, I, and D — can be realized with analog circuits.

## Project Objective

To design and simulate an analog PID controller using op-amps to:

- Understand the behavior of P, I, D components individually
- Observe the effect of tuning PID parameters on the system response
- Explore the implementation of control theory concepts in hardware-level circuits

## Circuit Overview

![image](https://github.com/user-attachments/assets/c77fd868-6ace-4eb0-a26b-1ebfe6f05528)

The circuit contains the following blocks:

1. **Buffer Stage (U1):** Isolates the input 

![image](https://github.com/user-attachments/assets/ab3ac46d-39b4-4e76-858d-c12b69c4707b)

2. **Proportional Block (U2):** Scales the input linearly

![image](https://github.com/user-attachments/assets/5a9f8f7c-beee-4669-860e-f0541e88dbd8)

3. **Integrator Block (U3):** Integrates the input using RC network

![image](https://github.com/user-attachments/assets/abd517fd-4053-4e85-a228-f111bdec612f)

4. **Differentiator Block (U4):** Derives the rate of change

![image](https://github.com/user-attachments/assets/89ac1c2a-30c4-463e-aae4-577a420b7611)

5. **Summing Amplifier (U5):** Combines all three outputs

![image](https://github.com/user-attachments/assets/7e210b59-692f-45ee-b448-ecdf2b691b64)

6. **Low-pass Filter:** Smoothens the output signal

![image](https://github.com/user-attachments/assets/1f1c0870-23b1-4fc7-a765-6f7037e6ffdf)

### Input

- A step voltage input is applied to test the system’s response.

### Output

![image](https://github.com/user-attachments/assets/0e054077-334c-4389-96ab-e3c0d6d2db27)

- Final PID-controlled output is taken after the summing and filtering stages.
- Feedback path is also modeled for potential closed-loop analysis.

## Key Learnings

- Modeled proportional, integral, and derivative control behavior using analog components
- Tuned resistor and capacitor values to see real-time effect on the system's response
- Gained practical understanding of PID tuning principles (Kp, Ki, Kd)
- Applied theoretical control system knowledge in a circuit simulation tool
