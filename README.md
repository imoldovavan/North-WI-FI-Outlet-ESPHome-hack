# North WI-FI Outlet ESPHome hack (Model: SWA1)

![](https://github.com/imoldovavan/North-WI-FI-Outlet-ESPHome-hack/blob/main/Pics/MainBox.jpg)

I bought these real cheap from Marcs for $3.99 and they use an ESP8266EX that I was able to program using CON2.

Once you crack the case open you can see the CON2 on the left side pcb board. This board also contains the ESP8266EX chip on the back side.
![](https://github.com/imoldovavan/North-WI-FI-Outlet-ESPHome-hack/blob/main/Pics/EnclosureOpen.jpg)

![](https://github.com/imoldovavan/North-WI-FI-Outlet-ESPHome-hack/blob/main/Pics/ProgrammingConnector.jpg)

Connect your favourite USBtoSerial adapter to CON2 and remember that RXD from adapter connects to TXD at CON2 and so on...
To get the ESP8266EX into programming mode ground pin GPIO00 and then insert the USBtoSerial into your computer.
After about 5 seconds disconnect the GPIO00 pin from the ground and you are able to upload the bin file. I used TASMOTIZER for this.

I provided the yaml file for this so you can figure out from that what pins are used.
- GPIO 13 - Push Button
- GPIO 05 - Relay and D3 led
- GPIO 04 - D1 led

Tasmota template for this is:
{"NAME":"North_Outlet","GPIO":[1,0,1,0,288,224,0,0,1,32,1,1,0,0],"FLAG":0,"BASE":18}
