# Installing the ESP32 board in Arduino IDE
* In your Arduino IDE, go to File> Preferences
* Enter the following into the “Additional Board Manager URLs” field: https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
 	Then, click the “OK” button:
* Open the Boards Manager. Go to Tools > Board > Boards Manager…
* Search for ESP32 and press install button for the “ESP32 by Espressif Systems“


# ESP32 Web Server
## This is an example of a web server controlling two LEDs connected to the ESP32 :

**provided the code that creates the ESP32 web server. Open the Arduino File, but don’t upload it yet. You need to make some changes to make it work for you.**

**You need to modify the following lines with your network credentials: SSID and password. The code is well commented on where you should make the changes**

`// Replace with your network credentials`
`const char* ssid     = "REPLACE_WITH_YOUR_SSID";`
`const char* password = "REPLACE_WITH_YOUR_PASSWORD";`

**Now, you can upload the code and and the web server will work straight away. Follow the next steps to upload code to the ESP32:**
*  Plug your ESP32 board in your computer;
*  In the Arduino IDE select your board in Tools > Board (in our case we’re using the ESP32 DEVKIT DOIT board);
*  Select the COM port in Tools > Port.
*  Press the Upload button in the Arduino IDE and wait a few seconds while the code compiles and uploads to your board.
*  Wait for the “Done uploading” message.


**-After uploading the code, open the Serial Monitor at a baud rate of 115200,**

**Press the ESP32 EN button (reset). The ESP32 connects to Wi-Fi, and outputs the ESP IP address on the Serial Monitor. Copy that IP address, because you need it to access the ESP32 web server.**


**-To access the web server, open your browser, paste the ESP32 IP address,**

**If you take a look at the Serial Monitor, you can see what’s happening on the background. The ESP receives an HTTP request from a new client (in this case, your browser).**

