# Retina-Display-eDP-Adapter-For-UP-Board
This project contains the design files for an eDP adapter and backlight driver for iPad 3 retina displays. These have  2,048 by 1,536 (2K) resolution and are 9.7 inch in diagonal. They can be ripped out of bricked or defective ipads or bought as new replacement parts for about 40$. With an adapter such as this one http://abusemark.com/store/index.php?main_page=product_info&products_id=53&zenid=li1so9u2k8e7n3u8q3j7j0uqg2 you should be able to use 7.9 inch iPad mini screens too. Capacitive touch overlays for the 9.7 inch screens with i2c to USB converters can be found on aliexpress.

The adapter and backlight driver board is based on the Adafruit Qualia driver (https://learn.adafruit.com/qualia-high-res-displayport-desktop-monitor?view=all#overview). The PCB has been made smaller and the 3.3V buck regulator, ATtiny backlight control as well as the bulky display port connector have been removed since most single board computers already provide 3.3V as well as backlight control. The board can be used for any single board computer with eDP interface by soldering bare wires to the appropriate connector. I'm using this with an UP core with Windows 10. After some automatic driver installations in the background, the PWM dimming function started to work perfectly well. The retina display connectors can be found on ebay and are quite cheap. And yes, they can be hand soldered. Just use enough good quality flux.

![UP_with_retina](https://github.com/BigCorvus/Retina-Display-eDP-Adapter-For-UP-Board/blob/master/driverPCBretinaWithUPcore.jpg)

![UP_with_retina_working](https://github.com/BigCorvus/Retina-Display-eDP-Adapter-For-UP-Board/blob/master/UPcoreWithRetina.jpg)


A .brd file for a connector for CN31 of the UP board or UP core is included, which can be manufactured by the new OSH Park flex service and costs next to nothing. The 5 differential pairs as well as wires for the 3.3V supply and control lines are soldered directly to the flex PCB using 30AWG solid core wires. Note that the flex PCB seems to be a little too thick for the connector to close properly, but the friction fit seems to be sufficient. 

![UP_eDP_connector](https://github.com/BigCorvus/Retina-Display-eDP-Adapter-For-UP-Board/blob/master/eDP_connector_UP.png)

