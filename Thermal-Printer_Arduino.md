# Thermal Printer with Arduino

Also known as receipt printers, you simply need a 3.3V to 5V TTL serial output from your microcontroller to print text, barcodes, bitmap graphics, even a QR code!

These printers use very common 2.25" (58mm) wide thermal paper, available at hackSpace. 


----
## HARDWARE

- Arduino Uno

- Thermal Printer

- 5V 2.4A Power Supply (Thermal Printer specific)

- Printing paper
  
- Jumping wires
  
----
## WIRING

Printer Black Wire  = Arduino GND
Printer Yellow Wire = Arduino pin5 (data IN to the printer (RX))
Printer Green Wire  = Arduino pin6 (data OUT of the printer (TX))

----
## CODE and INSTRUCTIONS

### 1. FIRST TEST

- Follow this [instructions for a first test](https://learn.adafruit.com/mini-thermal-receipt-printer/first-test)

### 2. INSTALL LIBRARIES

- [Download the Thermal Printer Library](https://github.com/kingston-hackSpace/Thermal_Printer/raw/refs/heads/main/Adafruit-Thermal-Printer-Library-master.zip)

- Unzip the library folder

- Locate the folder as follows:

  - Mac: /Documents/Arduino/Libraries
  
  - Windows: MyDocuments\Arduino\libraries
  
  - Linux: /sketchbook/libraries


----
## READ MORE

This tutorial is based on: [Adafruit Thermal Printer tutorial](https://learn.adafruit.com/mini-thermal-receipt-printer/overview)
