# Retina-Display-eDP-Adapter-For-UP-Board
This project contains the design files for an eDP adapter and backlight driver for ipad 3 retina displays. These have  2,048 by 1,536 resolution and are 9.7 inch in diagonal.

The adapter and backlight driver board is based on the Adafruit Qualia driver (https://learn.adafruit.com/qualia-high-res-displayport-desktop-monitor?view=all#overview). The PCB has been made smaller and the 3.3V buck regulator, ATtiny backlight control as well as the bulky display port connector have been removed since most computers provide 3.3V as well as backlight control. The board can be used for any single board computer with eDP interface by soldering bare wires to the appropriate connector. I'm using this with an UP core, although I have yet to figure out how the dimming works.

A .brd file for a connector for CN31 of the UP board or UP core is included, which can be manufactured by the new OSH Park flex service and costs next to nothing. The differential pairs as well as wires for the 3.3V supply and control lines are soldered directly to the flex PCB using 30AWG solid core wires. Note that the flex PCB seems to be a little too thick for the connector to close properly, but the friction fit seems to be sufficient.

