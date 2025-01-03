Up-Down Counter

This repository contains the RTL (Register Transfer Level) design and testbench code for a 4-bit synchronous up-down counter. The counter is implemented using Verilog and simulates counting operations based on a clock signal, reset signal, and a direction control signal (UpDown).

Overview:

The up-down counter is a fundamental digital design that increments or decrements its count based on the control signal UpDown. It is commonly used in applications such as digital timers, frequency dividers, and control systems.

Features:

4-bit counter (range: 0–15).
Synchronous design with a clock (Clk) and asynchronous reset (reset).
Up-counting mode (UpDown = 1) and down-counting mode (UpDown = 0).
Roll-over and roll-under behavior:
Up-count: Rolls over from 15 to 0.
Down-count: Rolls under from 0 to 15.

RTL Code Description:

The RTL code defines the behavior of the 4-bit up-down counter. Key highlights include:

Inputs:

Clk: Clock signal.
reset: Asynchronous reset signal.
UpDown: Direction control signal.
Output:
Count: 4-bit counter value.

Behavior:

When reset is asserted, the counter resets to 0.
When UpDown is high, the counter increments.
When UpDown is low, the counter decrements.

Testbench Description:

The testbench verifies the functionality of the up-down counter by generating:
A clock signal (Clk) with a 20 ns period.
Various scenarios for reset and UpDown to test counter operation under different conditions.

Simulation scenarios include:

Counter in up-count mode.
Counter in down-count mode.
Resetting the counter during operation.
