# North-WI-FI-Outlet-ESPHome-hack

![](https://github.com/imoldovavan/North-WI-FI-Outlet-ESPHome-hack/blob/main/Pics/MainBox.jpg)
I bought these real cheap from Marcs for $3.99 and they use an ESP8266EX that I was able to program using CON2.
![](https://github.com/imoldovavan/North-WI-FI-Outlet-ESPHome-hack/blob/main/Pics/ProgrammingConnector.jpg)

To get the ESP8266EX into programming mode ground pin GPIO00 and then insert the USBtoSerial into your computer.
After about 5 seconds disconnect the GPIO00 pin from the ground and you are able to upload the bin file. I used TASMOTIZER for this.

I provided the yaml file for this so you can figure out from that what pins are used.
GPIO 13 - Push Button
GPIO 05 - Relay and D3 led
GPIO 04 - D1 led
