# Frequency-Divider-circuit
I've designed this"Frequency Divider Circuit" using Xilinx ISE 14.7. The goal of this project was to design the hardware schematic that takes a 100 MHz clock as input and gives the output frequency totally based on the mode selected by the user.  The designed sequential circuit can convert 100 MHz frequency to 1 Hz, 100 Hz, 1 kHz, and 1MHz frequencies..
As the Asynchronous Up-Counter behaves as an f/2 divider circuit after each flip flop, I used this concept in this project to achieve the desired output.

It takes the following Inputs:

1. Clock = 100 MHz (Time Period = 10 ns)
2. Output Frequency Selector, Sel(1:0) where,
Sel = 00 will give 1 Hz frequency as output
Sel = 01 will give 100 Hz frequency as output
Sel = 10 will give 1 KHz frequency as output
Sel = 11 will give 1 MHz frequency as output
3. There's a CLEAR pin too to set the Initial Output Values of all the JK flip flops to 0.

For Example, if the user gives Sel = 11, Clock with a time period of 10 ns then the output frequency will be 1 MHz (approx.)
