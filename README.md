# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

/* write all the steps invloved */

**PROGRAM**

module EXP12DE(clk, rst, count);
input wire clk;
input wire rst;
output reg [3:0] count;

always @(posedge clk or posedge rst)
begin
	if(rst)
		count <= 4'b0000;
	else
		count <= count + 1;
end
endmodule
/* Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.

Developed by:Shreenidhi S
RegisterNumber: 212225040410
*/

**RTL LOGIC FOR 4 Bit Ripple Counter**

<img width="1068" height="388" alt="Screenshot 2026-05-21 201414" src="https://github.com/user-attachments/assets/a9999b2d-0e21-498d-872e-a0737063dd55" />


**TIMING DIGRAMS FOR 4 Bit Ripple Counter**

<img width="1066" height="553" alt="Screenshot 2026-05-21 201426" src="https://github.com/user-attachments/assets/f2257425-bea5-4e4a-8a4d-f3f6c9c41c3f" />


**RESULTS**
Thus implementing 4 Bit Ripple Counter using Verilog and validating their functionality using their functional tables is done successfully.
