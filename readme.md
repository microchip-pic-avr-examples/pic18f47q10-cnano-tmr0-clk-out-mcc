<div id="readme" class="Box-body readme blob js-code-block-container">
 <article class="markdown-body entry-content p-3 p-md-6" itemprop="text"><p><a href="https://www.microchip.com" rel="nofollow"><img src="images/MicrochipLogo.png" alt="MCHP" style="max-width:100%;"></a></p>

# PIC18F47Q10 Using TMR0 in 8-bit Mode and to Generate an Output Signal


## Objective:
This example describes how to configure TMR0 in 8-bit mode, using LFINTOSC as clock source. A GPIO pin will be
configured as output and a 125 Hz signal will be generated on the GPIO pin using the Peripheral Pin Select (PPS).
The code was generated using MPLAB Code Configurator.

## Resources:
- Technical Brief Link [(linkTBD)](http://www.microchip.com/)
- MPLAB® X IDE 5.30 or newer [(microchip.com/mplab/mplab-x-ide)](http://www.microchip.com/mplab/mplab-x-ide)
- MPLAB® XC8 2.10 or newer compiler [(microchip.com/mplab/compilers)](http://www.microchip.com/mplab/compilers)
- MPLAB® Code Configurator (MCC) 3.95.0 or newer [(microchip.com/mplab/mplab-code-configurator)](https://www.microchip.com/mplab/mplab-code-configurator)
- MPLAB® Code Configurator PIC10/PIC12/PIC16/PIC18 library v1.79.0 [(microchip.com/mplab/mplab-code-configurator)](https://www.microchip.com/mplab/mplab-code-configurator)
- PIC18F47Q10 Curiosity Nano [(DM182029)](https://www.microchip.com/Developmenttools/ProductDetails/DM182029)
- [PIC18F47Q10 datasheet](http://ww1.microchip.com/downloads/en/DeviceDoc/40002043D.pdf) for more information or specifications.

## Hardware Configuration:

The PIC18F47Q10 Curiosity Nano Development Board [(DM182029)](https://www.microchip.com/Developmenttools/ProductDetails/DM182029) is used as the test platform.

The following configurations must be made for this project:
- Clock
	– Oscillator Select: HFINTOSC
	– HF Internal Clock: 1 MHz
	– Clock Divider: 1
- Port
	- RC2 pin - Configured as digital output
- TMR0
	- TMR0 Enabled
	- Clock Prescaler: 1:1
	- Postscaler: 1:1
	- Timer mode: 8-bit
	- Clock Source: LFINTOSC
	- Synchronization: disabled
	- Timer interrupt: enabled
- Watchdog Timer: disabled

## Demo:
Run the code, an 125 Hz signal will be generated on the RC2 pin.

<img src="images/TMR0_clk_out_RC2.png" alt="Hardware Setup"/>