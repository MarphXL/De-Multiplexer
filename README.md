# CD74HC4067 - 16-Channel Analog/Digital Multiplexer/Demultiplexer

## Inhaltsverzeichnis
1. [x] [Inhaltsverzeichnis](#Inhaltsverzeichnis)
1. [x] [Beschreibung](#Beschreibung)
1. [x] [Technische Daten](#technische-daten)
   1. [x] [Datasheet](#datasheet)
1. [ ] [Hardware](#Hardware)
1. [ ] [Software](#Software)
1. [ ] [3D](#3D)
1. [x] [Where to buy](#Where-to-buy)
1. [x] [Abbildungen](#Abbildungen)
1. [x] [Credits](#Credits)

## Beschreibung
This is a breakout board for the very handy 16-Channel Analog/Digital Multiplexer/Demultiplexer CD74HC4067. This chip is like a rotary switch - it internally routes the common pin (COM in the schematic, SIG on the board) to one of 16 channel pins (CHANxx). It works with both digital and analog signals (the voltage can't be higher than VCC), and the connections function in either direction. To control it, connect 4 digital outputs to the chip's address select pins (S0-S3), and send it the binary address of the channel you want (see the datasheet for details). This allows you to connect up to 16 sensors to your system using only 5 pins!
Since the mux/demux also works with digital signals, you can use it to pipe TTL-level serial data to or from multiple devices. For example, you could use it to connect the TX pins of 16 devices to one RX pin on your microcontroller. You can then select any one of those 16 devices to listen to. If you want two-way communications, you can add a second board to route your microcontroller's TX line to 16 device's RX lines. By using multiple boards, you can create similar arrangements for I2C, SPI, etc.
The internal switches are bidirectional, support voltages between ground and VCC, have low “on” resistance and low “off” leakage, and to prevent crosstalk, perform “break-before-make” switching. The board also breaks out the chip's “enable” pin, which when driven high, will completely disconnect the common pin (all switches “off”).
 


## Hardware
### Technische Daten
* Modell:Multiplexer/Demultiplexer
* Typ:74HC 4067
* Temperaturbereich:-40 ... +85 °C
* Versorgungsspannung:2,0 ... 10,0 VDC
* Eingangsspannung Vi:0 ... 10 VDC
* Leistung:500 mW
* Eingangsspannung ViH:6,3 VDC
* Eingangsspannung ViL:0,5 VDC
* “On” resistance: 70 Ohms @ 4.5V
* 6ns break-before-make @ 4.5V
* Analog Input: C0-C15 16 channels
* Analog output: DIG
* Channel Control: S0-S3
* LCSC Part #: C6525 / C424181 / [C98457](https://lcsc.com/product-detail/Analog-Switches_TI_CD74HC4067SM96_CD74HC4067SM96_C98457.html/?href=jlc-SMT)
* EAN / GTIN: 9900001079047

### Datasheet
* [TI.com datasheet](https://www.ti.com/lit/ds/symlink/cd74hc4067.pdf)
* [snapshot](https://github.com/MarphXL/De-Multiplexer/blob/master/datasheet/cd74hc4067.pdf)
### EasyEDA
### Eagle
## Software
## 3D

## Where to buy
~ 6 EUR for 10pcs: [AliExpress](https://www.aliexpress.com/item/32821800330.html)

## Abbildungen
![HP4067](https://raw.githubusercontent.com/MarphXL/De-Multiplexer/master/images/HP4067_front.jpg)
![HP4067](https://raw.githubusercontent.com/MarphXL/De-Multiplexer/master/images/HP4067_back.jpg)

## Credits
* :+1: [arduino](https://github.com/arduino)
* :+1: [adafruit](https://github.com/adafruit)
* :+1: [sparkfun](https://github.com/sparkfun)
* :+1: [Watterott](https://github.com/watterott) and @awatterott for great SW, HW and products
* :+1: [atom](https://github.com/atom) 
* :+1: @ikatyang for the [emoji-cheat-sheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)
