# VHDL: Incorrect Signal Initialization
This repository demonstrates a common error in VHDL related to signal initialization and its effects on process behavior.  The bug involves improper handling of signal default values within a clocked process.

## Bug Description
The `my_entity` design uses a process to update the `data_out` signal based on `data_in`.  The problem arises in how the `internal_data` signal is initialized and used. The incorrect initialization can lead to unpredictable behavior in the initial clock cycles.