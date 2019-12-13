Step 1 - Getting arduino set to upload "bin" file to ESP8266
In your Arduino sketchbook directory, create tools directory if it doesn’t exist yet.
Unpack the ESP8266FS Zip file into the new tools directory (the path will look like <home_dir>/Arduino/tools/ESP8266FS/tool/esp8266fs.jar) 
Restart Arduino.
Open a new sketch file that you will use for the lights on DIYHUE and save it
Go to the sketch menu on the tool bar in arduino (choose Show Sketch Folder).
Create a directory named data and add the Bin file from the github for your lights WS2812B is - /bin/generic_WS2812B_Strip.bin

Step 2 uploading Bin file to SPIFFS on ESP8226
With the sketch open click on Tools and select "ESP8266 Sketch Data Upload" you will see SPIFFS complete message at bottom of arduino screen

Step 3: Upload sketch file to Arduino
Make sure you have loaded esp boards to arduino then select the board to upload to.
Open the "Generic_Ws2812_Strip.ino" file from Lights Master Zip and copy the content and paste into your sketch
Before uploading open serial monitor and ensure the Baud rate is the same as the Esp board. Once finished uploading it will tell you a IP address
Upload the Sketch to your board

Step 4:
When you plug in the board to your lights and power on you should see a running white light that means it is uploaded ok
When you see the green running light that means it is connected to WIFI
If you see a red running light it means WIFI failed
After white and green light navigate to the IP address you saw in the serial monitor via your browser
Here you will be able to rename your light and change some paramaters such as how many virtual lights, pixel count etc
Try turning the light on and off at this stage via the browser

Step 5:
Open Hue app and connect to pi bridge
Search for new lights
Your strip with given name should show - it will show a number of lights depending on what you set in step 4
Add lights to the room and away you go