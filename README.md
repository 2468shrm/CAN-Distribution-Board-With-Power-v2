# CAN-Distribution-Board-With-Power-v2

## Board Layout
![alt text](https://github.com/2468shrm/CAN-Distribution-Board-With-Power-v2/blob/main/Images/Board%20Layout.png?raw=true)

## Disclaimer
This board has not been fabricated or tested. It is to be considered
alpha and subject to bugs and errors. Use at your own risk. However the Gerbers
are provided should you want to fabricate your own.

## Introduction
This is a board created to simplify CAN wiring on FRC robots. It was created by the
mentors of FRC2468/2687/2689.

This board is a subset of the [CAN Distribution With Debug](https://github.com/2468shrm/CAN-Distribution-With-Debug) board.  The debug version of the board was created first and the
debug circuitry was removed while preserving the positions of the mounting holes and
connectors. This was done to share enclosures.

The board has 5 CAN connections and 3 power connections. The intended use is for
the CAN connections of either a swerve module or a WCD gearbox.
- Power
  - One connection upstream
  - One connection downstream
  - One connection to a local sensor (e.g. a CANcoder)
- CAN
  - One connection upstream
  - One connection downstream
  - One connection to a drive motor controller (Falcon 500, SPARK MAX)
  - One connection to a drive or steering motor
  - One connection to a CAN-connected sensor (CANcoder)

## CAN and Power Connections
The connectors for the CAN and power are WAGO 250-204s (X1, X2, X3, X4).

## Termination
The board contains a 2x2 header (J1) to allow for jumpers to be installed to enable
CAN termination.
- No jumpers means no termination
- One jumper provides 120 ohms termination (single end termination)
- Two jumpers provides 60 ohms termination (full termination)

Populating the termination circuitry is optional.

## Debug
THis board has two test point to probe CAN_H and CAN_L signal integrity.

# 3D Views of the Board
## Top
![alt text](https://github.com/2468shrm/CAN-Distribution-Board-With-Power-v2/blob/main/Images/CAN%20Distribution%20Board%20With%20Power%20v2%20Top.png?raw=true)

## Iso Front
![alt text](https://github.com/2468shrm/CAN-Distribution-Board-With-Power-v2/blob/main/Images/CAN%20Distribution%20Board%20With%20Power%20v2%20Iso.png?raw=true)

## Iso Back
![alt text](https://github.com/2468shrm/CAN-Distribution-Board-With-Power-v2/blob/main/Images/CAN%20Distribution%20Board%20With%20Power%20v2%20Iso2.png?raw=true)
