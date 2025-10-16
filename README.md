### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![WhatsApp Image 2025-10-15 at 10 06 01_c6bb109c](https://github.com/user-attachments/assets/31edf7a6-7d7b-443d-8e5d-5053673c3d21)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

 1. Type the program in Quartus software.
 2. Compile and run the program.
 3. Generate the RTL schematic and save the logic diagram.
 4. Create nodes for inputs and outputs to generate the timing diagram

**PROGRAM**

 <img width="1918" height="916" alt="Screenshot 2025-10-16 092058" src="https://github.com/user-attachments/assets/e8655393-e6e9-41ca-82a3-861e695e5fea" />


Developed by:G.SHAWN RONEL RegisterNumber:25005544
*/

**RTL LOGIC UP COUNTER**

**TIMING DIAGRAM FOR IP COUNTER**
![WhatsApp Image 2025-10-15 at 10 05 54_4f1d719b](https://github.com/user-attachments/assets/d4066f53-7bf7-402f-8939-6d48e9a2b6f2)

**TRUTH TABLE**

**RESULTS**
thus the basic logic gates are studied and the truth tables are verified
