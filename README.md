# ArduinoSimpleWebServer
First arduino project on wemos d1r1 wifi board. It connect to wifi network and after that we can turn on/off led via a webpage.

## initial steps to setup ESP8266 board(wemos d1 r1)

First: install Arduino IDE from [here](https://www.arduino.cc/en/Main/Software). Since I am using linux so I downloaded setup file for linux. 

Second: add wemos d1 r1 board configuration to IDE by going to **file->preferences** and add [http://arduino.esp8266.com/stable/package_esp8266com_index.json](http://arduino.esp8266.com/stable/package_esp8266com_index.json) url in **Additional Board manager URLs** field and then click ok. after that go to **tools->board->board manager** and search for esp8266 and install the latest version of package. Now go to **tools->board** and find wemos d1 r1 from board list and select that.

Setup is completed...

To test the setup run the example project by going to **file->examples->basics->blink** and click that. Now upload the code by clicking the right arrow button. If every things gone right then the in built led will start blinking. 

Error encountered by me: permission denied for /dev/ttyUSB0 
To solve this go to terminal and run the command **sudo chmod a+rw /dev/ttyUSB0**

Thats all for the first time... Now we can create new sketchboard and deploy various sketch.
