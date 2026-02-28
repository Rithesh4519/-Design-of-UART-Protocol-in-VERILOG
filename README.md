
##  Simulation
- Simulated using **Vivado xsim** (can also be run in ModelSim).
- TX testbench verifies UART frame generation.
- RX testbench verifies correct sampling and error detection.
- Loopback testbench connects TX → RX to validate end-to-end communication.


## FPGA Implementation
1. Add `uart_tx.v` and `uart_rx.v` to your Vivado project.
2. Map `tx` and `rx` signals to FPGA pins in `uart_fpga.xdc`.
3. Generate bitstream and program FPGA.


## PC Integration
- Use a terminal program (PuTTY, Tera Term, Arduino Serial Monitor).
- Configure baud rate (9600 or as parameterized).
- Type characters in PC terminal → FPGA RX receives them.
- FPGA TX sends characters → PC terminal displays them.


## Future Enhancements
- Support for higher baud rates (e.g., 115200).
- Parity bit implementation.
- FIFO buffering for TX/RX.
- Error logging and recovery mechanisms.


##  License
This project is open-source under the MIT License. Feel free to use, modify, and share.


##  Author
Rithesh
Student Electronics & Communication Engineering 
