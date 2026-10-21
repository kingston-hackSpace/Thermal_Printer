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

- Go to the Arduino Library Manager(top panel) and follow: Sketch → Include… Library → Manage… Libraries…

- At the search box, type: "Adafruit Thermal Printer Library"

- Find it and install it

### 3. TESTING CODE

- Open a basic example:

    File → Examples → Adafruit_Thermal Printer Library → A_printertest

- Upload this code (A_printertest) to your Arduino board

  - Troubleshooting: If your printer test page shows 'BAUDRATE: 9600', follow intructions [here](https://learn.adafruit.com/mini-thermal-receipt-printer/microcontroller)

### 4. FEATURES
    
- The thermal printer can do several things (demo in the A_printertest sketch). Look at the previous code and explore the features:

  - **Inverted text**: this is invoked by calling inverseOn() — you will get text that’s white-on-black instead of black-on-white. inverseOff() turns this off.

  - **Double height**: this makes text thats extra tall, call doubleHeightOn() — likewise, turn off with doubleHeightOff()

  - **Left/Center/Right justified**: this aligns text to the left or right edge of the page, or centered. You can set the alignment by calling justify('R') (for right-justified), justify('C') (for centered) or justify('L') (for left-justified). Left-justified is the default state.

  -  **Bold text**: makes it stand out a bit more, enable with boldOn() and turn off with boldOff()

  -  **Underlined text**: makes it stand out a bit more, enable with underlineOn() and turn off with underlineOff()

  -  **Large/Medium/Small text**: by default we use small, medium is twice as tall, large is twice as wide/tall. Set the size with setSize('L'), setSize('M') or setSize('S')

  -  **Line spacing**: you can change the space between lines of text by calling setLineHeight() where numpix is the number of pixels. The minimum is 24 (no extra space between lines), the default spacing is 32, and double-spaced text would be 64.

### 5. IMAGES

For printing images, follow this [Bitmap tutorial](https://learn.adafruit.com/mini-thermal-receipt-printer/bitmap-printing)

### 6. BAR/QR CODES

For printing bar codes and QR codes, follow this [bar codes and QR codes tutorial(https://learn.adafruit.com/mini-thermal-receipt-printer/barcode-printing)

----
## READ MORE

This tutorial is based on: [Adafruit Thermal Printer tutorial](https://learn.adafruit.com/mini-thermal-receipt-printer/overview)
