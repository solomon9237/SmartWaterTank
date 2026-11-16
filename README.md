# Smart Water Tank Monitoring and Control

A Logisim-evolution circuit that monitors water level, controls a pump, displays the level, and signals when the tank remains full.

## How it works
- Sensors `S0`–`S3` represent water levels from the bottom sensor to full.
- The circuit encodes the level as `00` (empty), `01` (25%), `10` (50%), or `11` (full).
- The pump runs when the tank is not full and stops when it is full.
- A 7-segment display shows the level as 0–3.
- The overflow alarm activates after three clock cycles at full and clears on a clock edge after the tank is no longer full.
- `RESET` clears the stored level on the next clock edge.

## Running
Open `Smart_Water_Tank_Control.circ` in Logisim-evolution 5.0.0. Select **Simulate** mode and the Poke tool to change inputs; click `CLOCK` to advance the circuit.

The submission PDF contains the system explanation, truth tables, Boolean equations, K-maps, and test scenarios.# SmartWaterTank
