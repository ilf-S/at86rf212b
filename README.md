Kicad project files for a 2 layer PCB with AT86RF212B transceiver. The board uses separated digital and analog ground planes on a 2 layer PCB design. Board has not been tested yet, so use with caution.


-2 Layer design
-4 Ground planes: Digital, Analog, Xtal & RF
 -- Digital handles all signals like SPI connection, IRQ, etc.
 -- Analog is mostly for things connected to the RF/Xtal, etc. but is confined bellow the IC QFN package. Consult the documentation, all analog ground pins are connected to the pads bellow the QFN.
 -- The RF is a separate plane connected to the IC by the two analog GND pins surrounding the RF_P/RF_N pins. Again consult the documentation
 -- The Xtal GND plane is connected to the IC with a single Analog GND pin and is hard grounded with via stitches. This hopefully will help with interference with the nearby IRQ pin. Capacitance could be an issue, though, might need some tweaking.

The rest is straight forward. Still not tested!
