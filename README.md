# compact-2-port-usb-charger-module

This project is a compact dual-port USB charger module designed to convert a 12V input into two regulated 5V USB outputs. Each port can deliver up to 15W, or 5V at 3A, using a synchronous buck converter and USB power-distribution switches.

The design focuses on stable power delivery, current limiting, USB charging control, compact PCB layout, and clean routing for power and differential USB lines.

## Key Features

- 12V input to regulated 5V USB output
- Two USB-A charging ports
- Up to 3A output current per port
- LM73606 synchronous buck converter
- TPS2549 USB power-distribution switch for each port
- Current limiting and port power control
- Fault indication using LEDs
- Compact PCB layout for pluggable module design
- Differential pair routing for USB D+ and D- lines
- Power and ground copper polygons for low-impedance routing

## Major Components

| Component | Function |
|---|---|
| LM73606 | 6A synchronous buck converter for 12V to 5V conversion |
| TPS2549 | USB power switch and port controller |
| USB-A Connectors | Charging outputs for connected devices |
| LED Indicators | Charging and fault status indication |
| Input Connector | 12V input, ground, and control connection |

## Design Approach

The LM73606 buck converter steps down the 12V input to a stable 5V rail. Each USB port uses a TPS2549 power switch to manage charging behavior, current limiting, and fault protection.

The PCB layout is designed to stay compact while still supporting high-current routing. Wide traces, larger vias, and copper polygons are used for 5V and ground nets to reduce impedance and improve power delivery. USB D+ and D- lines are treated as differential pairs to support proper signal routing.

## Project Files

- [Schematic Diagram](https://github.com/harinibabu63/compact-2-port-usb-charger-module/blob/main/USB%20charger%20module%20schematic.png)
- [PCB Layout](https://github.com/harinibabu63/compact-2-port-usb-charger-module/blob/main/USB%20charger%20Module%20PCB.png)
- [3D Board View]()
- [Bill of Materials]()

## What I Learned

- Buck converter-based power supply design
- USB power switching and current limiting
- Compact PCB layout planning
- High-current trace routing
- Differential pair routing for USB signals
- Power and ground polygon usage
- BOM preparation and component selection
