On a daily basis, people use weather forecasts to determine what to wear on a given day or to plan travel or events

However, it only tells temperature in a relatively large range. Sometimes we need environmental parameters in a specific place like a fishpond, greenhouse, an open field, etc. Here I want to know the exact temperatures during a day on my terrace. So I decide to make a weather monitoring station that outputs the real-time data I need. 

I got this environmental sensor from DFRobot that can measure temperature, humidity, pressure, ambient light, and UV, which is well suitable for this project.

This summer is much hotter than previous ones, and many places got record-breaking temperatures of over 40℃. For the sake of convenience, I add a UART fiber optic transceiver module in the project for data transmission, so I don't need to go outside to view data all the time. 

Video coming soon!!!

projectImage
projectImage
projectImage
HARDWARE LIST
2
ESP32-E IoT Microcontroller
Link
1
Gravity: High Accuracy Temperature, Humidity, Pressure, Ambient Light and UV Sensor
Link
1
OLED Transparent Display
Link
2
UART Fiber Optic Transceiver Module
Link
1
SC-SC Single Mode Duplex Fiber Jumper (50m)
Link
1
Lithium Battery Charger
Link
2
3.7V Battery
Link
Hardware Connection
 

Display End：

projectImage
Sensor End：

projectImage
Assembly
 

Display End：

We need to design the housing first and 3D print it.

projectImage
Then connect all the modules according to the connection diagram.

Now we put hardware modules into the housing. Install ESP32 main controller first (please be careful during installation to avoid wire disconnection), then fix the battery on the top of the housing with glue.

projectImage
And install the UART fiber optic transceiver module on the bottom of the housing.

projectImage
Connect ESP32 to the cable that comes with the OLED transparent display, and tidy it up.

projectImage
Connect the cable to the display converter.

projectImage
projectImage
Next, we need to make a frame for the display. 

Draw the frame and laser cut two acrylic sheets according to the drawing.

projectImage
projectImage
Then put the display between the two sheets and join them with super glue.

projectImage
projectImage
Install the display frame on the housing, and the display end is done.

projectImage
Sensor End：

Design the housing for the sensor end.

projectImage
In the same way, connect all the modules according to the connection diagram.

Then we need to make the battery charger and the sensor adhere to the fiber optic transceiver.

Use glue to fix the charger; thread a nylon hex bolt through the upper-right holes of the sensor and transceiver and fasten it with a fit nut to fix the sensor.

projectImage
Fix the battery on the transceiver with glue, and thread nylon hex bolts through the holes in the two corners of the fiber optic module and fasten them so that the structure can keep steady on flat.

projectImage
As shown in the figure below, the structure has three layers.

projectImage
Now put the structure into the housing.

projectImage
And put on the cover.

projectImage
Finally finished! Let's have it a go.

 

Test
Now we place the tripod holding the sensor end outside.

projectImage
Connect the sensor end to the display end with optic-fiber cable.

projectImage
Then we can view the real-time temperature and humidity data at the display end.

If there is no data shown on your display, try exchanging pins TX and RX of one end.

projectImage
 

With the multi-functional environmental sensor, the weather station can also measure air pressure, ambient light and UV intensity besides temperature and humidity, so we can use our brains to make the most of it. For example, we can apply it to greenhouse planting monitoring, fishpond status view, laboratory experiments, etc. But we need to take good care of the display lest a backlight bleed may occur at the damaged corner and thus affect display effect.

 

Thanks for reading, feel free to leave your comments if you have any other good ideas!
