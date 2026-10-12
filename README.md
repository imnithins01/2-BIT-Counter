# 2-BIT-Counter
2 Bit Counter using 555 Timer Clock,Master slave flipflop and 7 segment display.
# 555 Timer-Based 2-Bit Digital Counter

## Overview
A hardware-based college hackathon project demonstrating a 2-bit digital counter using a 555 timer IC, NAND/NOT-based flip-flop logic, decoding gates, and a common-cathode 7-segment display.

The reported hardware output cycles through decimal digits **0, 1, 2, and 3**.

## Block-Level Signal Flow
`555 timer clock pulses → flip-flop/state logic → 2-bit binary outputs → decoding logic → common-cathode 7-segment display`

## Intended State Mapping

| Count step | Binary output (Q1 Q0) | Display |
|---|---|---|
| 1 | 00 | 0 |
| 2 | 01 | 1 |
| 3 | 10 | 2 |
| 4 | 11 | 3 |
| Next cycle | 00 | 0 |

*Confirm the Q1/Q0 labels against the final circuit wiring.*

## Hardware
- 555 timer IC
- NAND and NOT gates or corresponding logic ICs
- Components needed for the flip-flop stages
- Common-cathode 7-segment display
- Timer resistors and capacitor(s)
- Breadboard/circuit board, jumper wires, and suitable DC supply
- Current-limiting resistors and any interface components actually used

**Important:** The exact timer mode, component values, supply voltage, logic IC part numbers, and clock frequency have not been confirmed. They are intentionally not guessed here. Update this list after checking the actual circuit.

## Working Principle
1. The 555 timer supplies pulses that trigger counter state changes.
2. NAND and NOT gates implement the state-storage/flip-flop logic used in the circuit.
3. The two-bit counter represents four states: `00`, `01`, `10`, and `11`.
4. Decoding logic drives the segments needed to display digits 0–3.

For a common-cathode display, the common cathode is connected to the appropriate ground reference and a segment typically lights when its anode is driven HIGH through suitable current-limiting/interface circuitry. Verify the display pinout and wiring against its datasheet.

## Evidence
My own project related references:
- 555 timer circuit.png
- [Flip flop and 555 timer circuit.png](https://github.com/imnithins01/2-BIT-Counter/blob/73874b1f8792a92a47e90c6d623ca12946b48388/Flip%20flop%20and%20555%20timer%20circuit.png)
- [2 BIT K-map.jpeg](https://github.com/imnithins01/2-BIT-Counter/blob/13734c1804bcf97c3060ca23fcf104046993f76e/2%20BIT%20K-map.jpeg)
- `Flip flop and 555 timer bread circuit.png`
- [Circuit Board.jpeg](https://github.com/imnithins01/2-BIT-Counter/blob/b69b684c98f2c71c44520223e07bd3e3b93602dd/Circuit%20Board.jpeg)
- [2 BIT COUNTER Output Video.mp4](https://github.com/imnithins01/2-BIT-Counter/blob/028e686d9ad53c388f490749ec35cf56311f73ac/2BIT%20COUNTER%20Output%20Video.mp4)
- [0 Output.jpg](https://github.com/imnithins01/2-BIT-Counter/blob/e56649fd1fce9ce3c0ca1e307613868c1bb1095f/0%20Output.jpg)
- [1 Output.jpg](https://github.com/imnithins01/2-BIT-Counter/blob/14889ad2008044e885a601405e80b774a97a41a1/1%20Output.jpg)
- [2 Output.jpg](https://github.com/imnithins01/2-BIT-Counter/blob/bc9cf81809725b3fb3cee8ccdfe702da265247d6/2%20Output.jpg)
- [3 Output.jpg](https://github.com/imnithins01/2-BIT-Counter/blob/dd66cc1bee386100bdb46a02d815546be684cf2e/3%20Output.jpg)
- [555_timer_2_bit_counter_project_report.pdf](https://github.com/imnithins01/2-BIT-Counter/blob/795c7e6cb8022eedc2fd3d8aa413885de0ee15a3/555_timer_2_bit_counter_project_report.pdf)

## Learning Outcomes
This project provided practical exposure to ICs, clock pulses, digital logic, flip-flop state storage, binary counting, display interfacing, and hardware troubleshooting. It also involved learning unfamiliar concepts through online resources and guidance from college seniors and professors.

## Limitations / Details to Confirm
- 555 timer configuration (astable or monostable)
- Resistor and capacitor values
- Supply voltage and measured pulse frequency
- Logic IC part numbers and exact flip-flop topology
- Actual segment decoding truth table and pin connections

## Reference
Texas Instruments, NE555 product information and datasheet: https://www.ti.com/product/NE555
