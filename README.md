### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */

**PROGRAM**

![image](https://github.com/user-attachments/assets/6590f42b-8b85-4846-a30c-a917d2b5ab97)


/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by:Sarukesh D RegisterNumber:212224050044
*/

**RTL LOGIC UP COUNTER**

![image](https://github.com/user-attachments/assets/616e8be6-28d4-4586-aac6-84f408516779)


**TIMING DIAGRAM FOR IP COUNTER**

![image](https://github.com/user-attachments/assets/5eee487b-5fb9-402a-b9f2-e646cb3ca81a)


**TRUTH TABLE**

![image](https://github.com/user-attachments/assets/9b8fe2e5-e8be-4a95-ad3d-cf495d48fa65)


**RESULTS**

Thus implemented a 4 bit synchronous up counter and validated its functionality.
