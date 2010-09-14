
This project is essentially a simple temperature controller or thermostat.

The temperature sensor used is a K-type thermocouple, interfaced to the microcontroller using a MAX6676 thermocouple compensator IC.
The use of a K-type thermocouple allows very high temperatures to be controlled. Thermistors and semiconducting sensors typically have much lower maximum operating temperatures than thermocouples.

This project was intended to be used to control an oven or hotplate for reflow soldering - however, it could be used for a multitude of other different applications.
Whilst thermocouples can withstand high temperatures, they also work perfectly well if you're working with lower temperature environments, too.

The microcontroller used is an ATmega328, running at 16 MHz. This microcontroller is compatible with the Arduino system, and the Arduino bootloader can be used on this board.
A 6-pin header for a standard FTDI cable is included on the board for use with the Arduino system - just as you would find on an Arduino Pro or Arduino Lilypad.
A standard 6-pin In-Circuit Programming header for the AVR is also present on the board.

A standard HD44780 16x2 LCD display is provided for the user interface, along with three pushbutton switches which can be used to navigate the menu or set the required temperature.
(Note that the software for this project has not been written just yet.)

The heating element load is controlled through a power relay with a maximum rating of 20 A at 240 VAC. This relay has two spade terminals on the top for the load connection.
A 2-pin header is also provided, connected in parallel with the relay coil. This allows an external relay to be connected, if a different relay is required.
Note that a relay with a 5 V coil must be used.

This also means that if the user is not comfortable with wiring mains voltage, they can use a pre-assembled relay-type device or have a more experienced person wire up the relay externally,
and simply connect up the low-voltage coil wires to the controller.

External unregulated DC power (around 7-15 V DC) is provided to the board via a standard DC barrel connector, and regulated down to 5 V on the board..

A small "prototyping area" is also provided on the PCB.

This board does contain a number of surface mount components. However, the resistors and capacitors are relatively large (0805), and there is only one IC, a SOIC 8-pin IC.
Therefore, this board is relatively easy to assemble, as far as surface mount based designs go. As such, it's a nice project to test a new SMD reflow oven or hotplate with, or, alternatively,
it's relatively easy to solder by hand.

