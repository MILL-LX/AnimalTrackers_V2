# Critter Connect 2
The project involves creating a wearable device equipped with *GPS* functionality. This device continuously accesses *GPS* coordinates to determine the user's location. Using these coordinates, it identifies the nearest predefined *Point of Interest* (POI). If this *POI* is within 100 meters of the user, the wearable lights up with a color associated with the animal species typical to that area.

## Features
- It allows to play the sound of the animal if the user is under 100 meters from the *POI* by pressing the button;
- If the user are not in the *Zone of Interest* (ZOI) the lights do not light up nor the *MP3* plays any sound;


## Circuit Design and Assembly

The circuit comprises four groups of components:

1. The microcontroller, which oversees the operation of other components.
2. The GNSS module, responsible for satellite communication to determine current location.
3. The MP3 module, along with the speaker and button, used to play animal sounds when inside the ZOI (Zone of Interest).

The assembly is depicted below:
![alt text](https://st.depositphotos.com/2274151/4841/i/450/depositphotos_48410095-stock-photo-sample-blue-square-grungy-stamp.jpg)

### Micontroller
The overseer of this operation is the micontroller **Seeed Studio XIAO ESP32C3** ( [Link to the website!](https://www.seeedstudio.com/Seeed-XIAO-ESP32C3-p-5431.html) ).

![XIAO ESP32-C3](https://media-cdn.seeedstudio.com/media/catalog/product/cache/bb49d3ec4ee05b6f018e93f896b8a25d/1/-/1-113991054-seeed-studio-xiao-esp32c3-45font_1.jpg)

Every other component is connected to the micontroler.

### GNSS module
This module is responsible to determine the current location of the user and communicate it to the micontroller.
The module used in this system is the **L76K GNSS Module** ( [Link to the website!](https://www.seeedstudio.com/L76K-GNSS-Module-for-Seeed-Studio-XIAO-p-5864.html) ).

![XIAO GNSS module](https://files.seeedstudio.com/wiki/Seeeduino-XIAO-Expansion-Board/GPS_Module/L76K/1-L76K-GNSS-Module-for-Seeed-Studio-XIAO-45font.jpg)

### MP3 module
The module responsible to play the animal sounds consists of three components: the **DFPlayer Pro** ( [Link to the website!](https://www.dfrobot.com/product-2232.html) ), the capacitive button ( [Link to website!](https://www.adafruit.com/product/1374) ) and the speaker connected to it.

![DFROBOT MP3 module](https://dfimg.dfrobot.com/store/data/DFR0768/DFR0768.jpg)
![DAFRUIT Standalone Momentary Capacitive Touch Sensor Breakout](https://cdn-shop.adafruit.com/970x728/1374-07.jpg)

The speaker to connect to the *MP3 player* can be any speaker.

