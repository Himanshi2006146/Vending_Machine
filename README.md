FPGA Vending Machine (Nexys 4) 🥤
A Verilog implementation of a vending machine on the Digilent Nexys 4 (Artix-7). Controlled by a Finite State Machine (FSM), it handles coin inputs, product selection, change dispensing, and displays the current balance on a 7-segment display.

✨ Features
Accepts 5₹ and 10₹ coins.

7 Products available (priced from 5₹ to 35₹).

Automatic change calculation.

Cancel button for full refund.

Multiplexed 7-segment display for balance tracking.

⚙️ Controls
SW[1:0] (coin): 01 = 5₹, 10 = 10₹

SW[4:2] (select): Selects product 0 to 6 (binary).

BTNC (cancel): Resets balance and refunds.

LEDs[6:0] (product): Lights up the dispensed product.

🚀 Quick Start
Open Xilinx Vivado and create a new project for Nexys 4 (xc7a100tcsg324-1).

Add vending_machine_7prod.v as a design source and set it as the Top Module.

Add your .xdc constraints file mapping the ports to the Nexys 4 pins.

Generate the Bitstream and program your board.
