# AutomaticHumidifer
An automatic humidifier that turns on the humidifier when the humidity level drops too low. The project uses the DHT11 Sensor and a 1.3 inch OLED display (I used the VMA 437) to show the temperature and humidity. An Arduino Uno is used as the microcontroller. Once it detects that the humidity has dropped to a certain level, the Arduino will complete the circut between the circult between the wall power and the humidifer through the relay switch. 

## Wiring 
* D0 = 13
* D1 = 11
* CS = 10
* DC = 9
* Reset = 8

DHT 11 Pin: A0

## Wire all VCC/5V/3V/Ground pins accordingly

### Icons On The Display
This part is fully optional but you can add an icon to the whitespace beside your data. You'll need to create a bitmap image (.bmp) and then convert it into a byte array (in memory format) in order for the picture to show up. The maximum dimensions of the image must be 50x50 px. Once you have the array paste it into the brainy_bitmap PROG_MEM array. 

