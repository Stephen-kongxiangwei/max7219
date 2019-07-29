# BBC micro:bit MakeCode editor extension for MAX7219 8x4 matrix LED modules

This extension works with single or multiple MAX7219 8x4 LED matrix display modules.

To import this extension, go to Advanced -> +extension and enter "MAX7219" in the search box, or copy/paste [https://github.com/Stephen-kongxiangwei/max7219]. Press enter and click the extension.
## Modules Wiring

For the module at the head of the chain, connect it to micro:bit as follows:

* VCC -> 3.3V or 5V (both works; using 5V make the LEDs a bit brighter, which is more preferable for some people.)
* GND -> GND
* DIN (MOSI or MO in SPI) -> default P15
* CS (LOAD pin) -> any pin you want (default P16)
* CLK (SCK in SPI) -> default P13
