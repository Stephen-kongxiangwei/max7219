# BBC micro:bit MakeCode editor extension for MAX7219 8x8 matrix LED modules

This extension works with single or multiple MAX7219 8x8 LED matrix display modules.

To import this extension, go to Advanced -> +extension and enter "MAX7219" in the search box, or copy/paste [https://github.com/Stephen-kongxiangwei/max7219]. Press enter and click the extension.
## Modules Wiring

For the module at the head of the chain, connect it to micro:bit as follows:

* VCC -> 3.3V or 5V (both works; using 5V make the LEDs a bit brighter, which is more preferable for some people.)
* GND -> GND
* DIN (MOSI or MO in SPI) -> default P15
* CS (LOAD pin) -> any pin you want (default P16)
* CLK (SCK in SPI) -> default P13

MISO or MI (default P14) is not used, but included anyway for SPI pins are reassigned together.

Of course, you can reassign these SPI pins in anyway you want; just use the setup block and remember to set the correct number of matrixs.
It's basicly the same as the first one, except all module's DIN connects to DOUT on the previous one. Be noted that in the wiring picture above the order of the pins are slightly different (for example, CS and CLK) from the module I used.

In my test the 3.3V power from micro:bit itself (90mA) is sufficient to power 4 chained MAX7219 modules. You may need more for a longer matrix chain.
