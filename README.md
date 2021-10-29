# RiazBot

‘Riaz-Bot’ USER MANUAL

‘Riaz-Bot’, named after Sketch House’s favourite security guard, is a creative computing project aiming to make the life of a security officer easier. By detecting noise above a set threshold, ‘Riaz-Bot’ will alert the user via an 8 by 8 LED panel and an LED bulb. This document is a step by step guide to building a ‘Riaz-Bot’ free of jargon, knowledge assumptions and accessible to the creative computing community in K204 and beyond.

1.1.1; Arduino Uno Set-Up

Plug the first Arduino Uno into laptop via USB 2.0 cable.
Open Arduino IDE software (see links).
Port the first board (Tools>Port>/dev/cu.Arduino-Uno).

1.1.2; Primary Breadboard Set-Up

Wire a jumper cable from the 5V output on the Uno to the ‘+’ column on the breadboard.
Wire a jumper cable from the GND output from ‘DIGITAL’ (left hand side of the Uno Board) to the ‘-‘ column.

2.1.2; 8 by 8 LED Panel Set-Up

Combining the primary breadboard with a secondary breadboard, plug the left half of the pins into J1-J8 of the primary board, and the other half into A1-A8 of the secondary board.

2.2.1; 8 by 8 LED Panel Primary Breadboard Wiring Set-Up

Wire a jumper cable from 5 from ‘DIGITAL’ to H1.
Wire a jumper cable from 3 from ‘DIGITAL’ to H2.
Wire a jumper cable from 11 from ‘DIGITAL’ to H3.
Wire a jumper cable from 12 from ‘DIGITAL’ to H4.
Wire a jumper cable from 2 from ‘DIGITAL’ to H5.
Wire a jumper cable from A0 from ‘ANALOG IN’ to H6.
Wire a jumper cable from 4 from ‘DIGITAL’ to H7.
Wire a jumper cable from 7 from ‘DIGITAL’ to H8.

2.2.2; 8 by 8 LED Panel Secondary Breadboard Wiring Set-Up

Wire a jumper cable from A3 from ‘ANALOG IN’ to C1.
Wire a jumper cable from A2 from ‘ANALOG IN’ to C2.
Wire a jumper cable from 8 from ‘DIGITAL’ to C3.
Wire a jumper cable from 10 from ‘DIGITAL’ to C4.
Wire a jumper cable from 6 from ‘DIGITAL’ to C5.
Wire a jumper cable from A1 from ‘ANALOG IN’ to C6.
Wire a jumper cable from 13 from ‘DIGITAL’ to C7
Wire a jumper cable from 9 from ‘DIGITAL’ to C8

3.1.1; Download FrequencyTimer2

Navigate to FrequencyTimer2 library on GitHub (see links).
Download .ZIP file (Green Code Button>Download ZIP).
Install library into Arduino IDE (Sketch>Include Library>Add.ZIP Library).



3.1.2; Coding the 8 by 8 LED

Access code (see links).
Remove all code from Arduino IDE.
Paste code into Arduino IDE.
Upload code (Top Left) to test LED.

4.1.2; Sound Sensor Set-Up

Plug the sound sensor into E20, E21, E22 on the primary breadboard (some sound sensors have 4 pins, inclusion of E24 may be necessary).
Wire a jumper cable from +20 to VCC (secondary Uno).
Wire a jumper cable from -20 to GND (secondary Uno).
Wire a jumper cable from 1 from ‘DIGITAL’ to OUT (If the sound sensor has AOUT and DOUT, use DOUT) (secondary Uno).

4.1.3; Connecting the LED Bulb

Plug the LED with the longer prong in E16 and the other into E18.
Wire a jumper cable from +16 to D16.
Wire a resistor from -18 to D18.

4.1.4; Coding the Sensor and Bulb

Access code (see links).
Connect the secondary Uno to Arduino IDE.
Remove all code.
Paste code from link into Arduino IDE.
Upload the code.

4.2.1; Common Problems

If the bulb does not turn on, then adjust the potentiometer on the sound sensor.
If all the bulbs on the LED Panel remain on, then swap the Row and Column numbers.
















Links;

Arduino IDE; https://www.arduino.cc/en/software
FrequencyTimer2; https://github.com/rookie/FrequencyTimer2
8 by 8 Code; https://docs.google.com/document/d/1TZfcZSpGhdmPf15O8Zm7_VW8LY1AftiR7ZDeBcJOQHE/edit
LED Code; https://docs.google.com/document/d/1LqUMCKC7Yf_ZNOMm0HGVC1CGUAmLJt9letnQ92g2i_U/edit?usp=sharing
