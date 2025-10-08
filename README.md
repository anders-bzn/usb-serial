# USB to RS232 serial converter
This is a galvanically isolated USB to RS2332 serial adapter. The repository includes project files for both a PCB and an enclosure.

## Short data:
- One USB-C connector and one DB25 D-SUB male connector
- Full ±12V voltage swing on the RS232 side
- Rx/Tx and RTS and CTS signals are available
- Galvanic isolation provided by the MAX22246
- USB to serial conversion handled by the CP2111
- Supported data formats:
    - Data bits: 5, 6, 7, and 8
    - Stop bits: 1, 1.5, and 2
    - Parity: Odd, even, mark, space and none
    - Baud rates from 300 to 921600

![USB serial adapter](usb-serial.png)

## Tools used
This project was created using:
- [KiCad 8.0](https://www.kicad.org/) and [kicad-jlcpcb-tools](https://github.com/Bouni/kicad-jlcpcb-tools) plugin for generating PCB and fabrication files
- [FreeCAD 1.0.2](https://www.freecad.org/downloads.php?lang=en) for 3D modeling the enclosure

## Assembly Instructions
To ensure easy and successful assembly, follow these steps:

1. Mount all surface-mount components.
All necessary files are included for ordering fully assembled PCBs (apart from through hole components) from JLCPCB.
2.  Mount all through-hole components.
This includes the 3mm green LED and the DC/DC converter.
3. Mount the D-SUB connector:
    * Place the PCB into the enclosure so the USB connector and LED aligned correctly.
    * Position the D-SUB connector and screw it in place using the #4-40 standoffs and solder it in place.
    * Disassemble the PCB and solder the other side of the D-SUB connector.
4. Final assembly
    * Reassemble the PCB in the enclosure.
    * Slide on the lid.
    * Secure the lid using 2 × M2.5 × 14mm countersunk machine screws.
