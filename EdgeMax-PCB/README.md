# EdgeMax-PCB

## Description

This project demonstrates a custom 4-layer PCB containing the STM32H743ZIT6 microcontroller. This board can be used for demanding edge embedded systems using multiple peripherals.

## Components

1. Microcontroller: STM32H743ZIT6
   - 1 MB total RAM and 2 MB Flash.
   - Up to 480 MHz clock speed.
   
2. USB Connectivity: USB4125-GF-A-0190
   - USB Type-C for data and power 

3. Power Supply: TPS62163DSGR
   - Step-down regulator for stable 3.3V output.
   - Support input voltage 3V to 17V.

4. Current and Power Monitor: INA219AIDCNR
   - Monitors the bus voltage.
   - Outputs digital values of current, power, shunt and bus voltage which the host can read via I2C.

6. Li-ion Battery Charger: BQ24074RGTR
   - Maximum charge current: 1.5A.
   - Input voltage: 4.35V up to 10.2V.
     
7. Headers:
   - GPIO, UART, SPI, I2C and JTAG headers for external connections.

8. Memory: RMLV0808BGSB-4S2#AA0
   - 8 Mbit SRAM storage.

9. Security: ATECC608B-MAHDA-S
   - Hardware-based encryption and storage for keys.
   - Support for cryptographic authentication.
  
10. NOR Flash Storage: MT25QL256ABA1EW9-0SIT
    - 256 Mbit Memory Size.
     
## Disclaimer

This project is currently in **testing phase**. The provided documentation is shared for prototyping and learning purposes. If you choose to manufacture and use the board, please proceed with care, as it has not yet been fully validated.

## Schematic and PCB Design

The board was designed using Altium Designer. Files from the PCB design can be found in the **hardware** folder for board manufacture. This folder includes:

- PCB Schematic 
- PCB Layout
- Gerber Files
- Assembly Files

Below is a 3D render of the PCB design:

<img width="1473" height="480" alt="image" src="https://github.com/user-attachments/assets/cc596208-b9fd-4163-9ff7-24b8d7d0c818" />

## How to Use

1. Power the board
   - Use a USB Type-C cable to power the board.
     
2. Microcontroller Programming:
   - Use STM32CubeIDE or any other platform to program the microcontroller.

3. Peripheral Access
   - Use the GPIO, SPI, I2C, UART and JTAG headers to connect peripherals.
