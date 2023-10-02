# meeeseeks
Arduino Code for ESP01S to run Mr. Meeeseeks Box

### Required Libraries
1. [WiFiManager](https://github.com/tzapu/WiFiManager)
2. [ArduinoJSON](https://github.com/bblanchon/ArduinoJson)
3. [DoubleResetDetect](https://github.com/jenscski/DoubleResetDetect)

### Wiring Diagram
1. Connect GND of ESP01 to GND of your battery
2. Connect VIN of ESP01 to 3v battery pack
3. Connect RST of ESP01 to S1 of your switch
4. Connect S2 of your switch to GND of your battery
5. Profit.

### Create a Webhook
1. Visit https://voicemonkey.io/ and register for an account
2. Follow the VoiceMonkey setup instructions \(Sign in with Amazon, Install the VoiceMoney Alex App, etc.)
3. Create a new "Routine Trigger" device and give it a fun name like, "Mr. Meeeseeks"
4. Click "APIv2" > "Routine Trigger API" in the sidebar
5. Select the trigger you just created.
6. Click "Copy URL"

### Operation
1. Double clicking the button should cause your Mr. Meeeseeks box to restart in Config Mode
2. Connect the the access point "MeeeseeksWifi"
3. If a portal doesn't appear, browse to http://192.168.4.1
4. Select your network and enter your wifi password to connect Mr. Meeeseeks to the internet
5. Paste in the URL from the "Create a Webhook" Step 6.
6. Click "Save"
7. Your Meeeseeks box will now reboot. Push the button to trigger your event.

### Screenshots
![A circuit diagram for the ESP01. Described in the wiring diagram section](diagram.png)