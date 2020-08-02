# AutomaticHumidifer
An automatic humidifier that turns on the humidifier when the humidity level drops too low. The project uses the DHT11 Sensor and a 1.3 inch OLED display (I used the VMA 437) to show the temperature and humidity. An Arduino Uno is used as the microcontroller. Once it detects that the humidity has dropped to a certain level, the Arduino will complete the circut between the circult between the wall power and the humidifer through the relay switch. 

## Wiring 
* D0 = 13
* D1 = 11
* CS = 10
* DC = 9
* Reset = 8

DHT 11 Pin: A0
Relay: 4

## Wire all VCC/5V/3V/Ground pins accordingly

### Hooking the relay up.
You'll need to find a humidifer that can turn on as soon as you plug it in (a static on and off switch no buttons). Cut the cable in half and plug on end into the D1 of the relay and the other into the D2 of the relay. Use a standard GPIO cable to plug the control pin onto the Arduino (default in code is 4). Wire the GND and 5V pins accordingly. 

### Icons On The Display
This part is fully optional but you can add an icon to the whitespace beside your data. You'll need to create a bitmap image (.bmp) and then convert it into a byte array (in memory format) in order for the picture to show up. The maximum dimensions of the image must be 50x50 px. Once you have the array paste it into the brainy_bitmap PROG_MEM array. 

## How To Build?
Download the .ino file and open using Arduino IDE. Upload to any microcontroller, but the code has only been tested using the Arduino UNO

![Picture](https://i.imgur.com/s27O8Kc.jpg)


