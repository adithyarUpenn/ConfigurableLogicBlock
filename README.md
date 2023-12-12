# Configurable Logic Block (CLB)

## Design Problem: 
<p>To design the circuit-level implementation of a Configurable Logic Block
(CLB) comprised of a single Basic Logic Element (BLE) using a Look-up Table (LUT).</p>

<p>The aim is to create a single design of a CLB with inputs –</p>
<p>•	Clock - Clk</p>
<p>•	Load (high when loading SRAM data)</p>
<p>•	Data (serial input of bitstream to load into SRAM)</p>
<p>•	LUT select <3:0></p>
<p>•	Output: Out</p>

<p>The CLB in an FPGA holds a custom truth table, which is loaded when the chip is powered up and implements the functionality of a Multiplexer (MUX). The CLB should be designed along with the control logic to load the SRAM cells with the desired truth table. The LUT inputs act as the address lines for a corresponding one-bit-wide RAM cell. </p>

<p>The LUT will have the following inputs – </p>
<p>•	data<15:0></p>
<p>•	addr< 3:0></p>
<p>•	output: Out.</p>

<p>When an FPGA is configured, the data bits of the LUT are loaded with ones or zeros based on what the desired truth table would be.</p>
