# Linkit ONE

[PDF](http://www.seeedstudio.com/wiki/images/d/da/Seeed_LinkIt_ONE_User_Manual.pdf)

The LinkIt ONE development platform is an open source, high performance board for prototyping Wearables and IoT devices. It is based on the world's leading SoC for Wearables, MediaTek Aster (**MT2502**) combined with high performance Wi-Fi (**MT5931**) and GPS (**MT3332**) chipsets to provide you with access to all the features of MediaTek LinkIt. It also provides similar pin-out features to Arduino boards, making it easy to connect various sensors, peripherals, and Arduino shields.

LinkIt One is an all-in-one prototyping board for IoT/wearables devices. Integrating GSM, GPRS, Wi-Fi, GPS, Bluetooth features into a basic Arduino form factor.LinkIt ONE is a co-design product by [Seeed Studio](https://www.seeedstudio.com/) and [ MediaTek](http://www.mediatek.com/). It brings together both parties' technology in open hardware and industrial leading reference designs for Wearables and IoT devices to create a powerful development board.

**Notes:** LinkIt ONE board comes with a lot of features and its SDK(Software Development Kit) is quite comprehensive. Read this document throughly once before using the board. Being a co-design product basic level Technical Support for hardware is provided at [ Seeedstudio LinkIt One Forum](http://www.seeed.cc/discover.html?t=linkit).Advanced Technical support is available at  [  MediaTek LinkIt One Forums](https://labs.mediatek.com/forums/forums/list.page).These forums have a good number of FAQs about this board.Please search solutions for your requirements/issues first before posting questions for saving your time. 

[![Get one now](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/150px-Get_One_Now_Banner.png)](https://www.seeedstudio.com/item_detail.html?p_id=2017)


## Features

- Includes ARM7 EJ-S™, GSM, GPRS, Wi-Fi, Bluetooth BR/EDR/BLE, GPS, Audio codec, and SD card connector on a single development board.
- Pin-out similar to Arduino boards, including Digital I/O, Analog I/O, PWM, I2C, SPI, UART and power supply, compatible with Arduino.
- Provides various interfaces for connecting to most sensors, peripherals, Groves, and other widgets.
- You are what you wear. Using LinkIt ONE together with MediaTek LinkIt SDK (for Arduino) you will be able to easily turn your ideas into practical prototypes and make them a reality with the Seeed productization and agile manufacturing service.


## specifications

|Parameter   |Value          |
|:------|:-----------------|
|Chipset|	MT2502A (Aster, ARM7 EJ-S (TM) )|
|Clock Speed|	260MHz|
|Dimensions|	3.3x2.1 inches|
|Flash|	16MB|
|RAM|	4MB|
|DC Current Per I/O Pin|	1mA|
|Analog Pins|	3|
|Digital Output	|3.3V|
|Analog Input|	5V|
|UART|	Software based(**Serial**) ,also known as USB Modem Port and Hardware Serial(**Serial1**, D0&D1)|
|SD Card|	Up to 32GB(Class 10)|
|Positioning|	GPS(MT3332)|
|GSM|	850/900/1800/1900 MHz|
|GPRS|	Class 12|
|Wi-Fi|	802.11 b/g/n|
|Bluetooth|	BR/EDR/BLE(Dual Mode)|

## Hardware Overview

![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/1000px-LinkItONE_RESOURCE.png)

### Configuration Switches
There are 3 slide switches on LinkIt ONE which are used to configure the function/working mode :

![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/300px-LinkIt_ONE_Wiki_Button.jpg)

|Switch No.|	Functionality|	Position 1 - Functionality|	Position 2 - Functionality|
|:------|:-----------------|:-----------------|:-----------------|
|1|	Program Mode|	**MS**： In this position, when connected to PC, LinkIt One board will be shown as 10MB USB drive. The program will not execute in this mode. Any file that is copied to this drive can be read via the code.|	UART：This position is used to set the board to program mode. Firmware can be uploaded in this mode.|
|2|	Power|	**BAT**： Board powered by Li-ion Battery. To charge battery, set the switch to this position and connect the board to PC.|	**USB**：Board powered by USB port. Set the switch to this position when there is no battery connected to program the board.|
|3|	SD/SPI|	**SPI**：This position allows access of external SPI pins (D10 - D13)	|**SD**：This position allows the code to access SD card. This mode also disables access of SPI pins (D10-D13).|

**Note** that DO take care as you handle USB micro type-B socket, or you might break the socket off.

## Getting started

### Procedure Overview
|No.|	Step	|Read more|
|:------|:-----------------|:-----------------|
|1|	Install Arduino IDE 1.5.7 Beta (Windows or MAC OS X version)|	[ here](http://www.seeedstudio.com/wiki/LinkIt_ONE#Installing_Arduino_IDE)
|2|		[ Register on MediaTek Labs](http://labs.mediatek.com/dpRegister/create).	| |
|3|	Download [ Linkit Developer's Guide](http://labs.mediatek.com/fileMedia/download/5fed7907-b2ba-4000-bcb2-016a332a49fd) and read.	||
|4|	Install [ LinkIt SDK](http://labs.mediatek.com/site/znch/developer_tools/mediatek_linkit/sdk_intro/index.gsp) for Arduino IDE (Windows or MAC OS X).|	[ here](http://www.seeedstudio.com/wiki/LinkIt_ONE#Installing_Mediatek_LinkIt_ONE_SDK)|
|5|	Install LinkIt ONE drivers.|	[ here](http://www.seeedstudio.com/wiki/LinkIt_ONE#Installing_Drivers)|
|6|	Update the on-board firmware version.|	[ here](http://www.seeedstudio.com/wiki/LinkIt_ONE#Updating_Firmware)|
|7|	Open Arduino IDE, Select LinkIt ONE board and start coding.|	[ here](http://www.seeedstudio.com/wiki/LinkIt_ONE#Uploading_Code)||
|8|	Connect GSM, GPS and WiFi/BT antennae to LinkIt One board|	[ here](http://www.seeedstudio.com/wiki/LinkIt_ONE#Connecting_Antennae)|
|9	|Insert SIM and Micro SD Card|[ here](http://www.seeedstudio.com/wiki/LinkIt_ONE#Inserting_SIM_Card_and_SD_Card)|
|10	|Explore examples and Happy making!|

### Installing Arduino IDE
[ Download latest Arduino IDE](https://www.arduino.cc/en/Main/Software) .For more advanced topics, follow MediaTekTM[  instructions](http://labs.mediatek.com/site/znch/developer_tools/mediatek_linkit/sdk_intro/index.gsp).
 
### Installing Mediatek LinkIt ONE SDK
- Download [  LinkIt SDK for Arduin](http://labs.mediatek.com/site/znch/developer_tools/mediatek_linkit/sdk_intro/index.gsp).At the time of writing this guide, **v1.1.11** Windows SDK (Beta) was used. Read the video guide for Windows OS and MAC OS X platforms  [ here](http://labs.mediatek.com/site/znch/developer_tools/mediatek_linkit/get-started/index.gsp)
- Extract the downloaded files to Arduino IDE folder.
- Double-Click the .EXE file and install.
- With the installation of LinkIt ONE SDK, Arduino IDE works a LinkIt ONE IDE.
### Installing Drivers
- Disable **Driver Signature Enforcement** if you are using Windows 8/8.1 OS. Read[instructions](http://www.seeedstudio.com/wiki/Download_Arduino_and_install_Arduino_driver#Installing_drivers_for_the_Seeeduino_with_window8)
- Put the MS/UART slide switch to UART position and connect LinkIt ONE to PC.
- Open Device Manager, the following COM ports will be displayed.
- 
![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/LinkIt_ONE_Wiki_Temp1.jpg)
- Install driver from ..\LinkIt_ONE_IDE\drivers\mtk folder.
- After installing drivers, Device Manger should display the following two ports:

   **MTK USB Debug Port** used for uploading code.
 
  **MTK USB Modem Port** used for printing message, such as Serial.println()
  
![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/LinkIt_ONE_Wiki_Temp2.jpg)  
**NOTE:** There is no official Windows 10 driver yet. Windows 10 users can manually select the Windows 7 driver files from \LinkIt_ONE_IDE\drivers\mtk from Device Manager. This is known to work on few PCs.

### Updating Firmware
The firmware of LinkIt ONE board needs to be updated once in a while. Latest LinkIt ONE SDK comes with a version of firmware.
- Before starting the firmware update, make sure the slide switches are in proper position ( **MS/UART** should be in **MS** position. **USB/BAT** in **USB** position):

![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/LinkItONEUpdateFirmware2.jpg)  
- Run FirmwareUpdater.exe application from ..**\LinkIt_ONE_IDE\hardware\tools\mtk** folder.

![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/400px-LinkItONEUpdateFirmware.jpg)  
- Click the button and then connect LinkIt ONE to PC. Wait for 1 minutes for the update to complete successfully.

![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/400px-LinkItONEUpdateFirmware_ok.jpg)  
### Uploading Code (Blinky)
- The slide switches should be configured for firmware upload (i.e Put MS/UART in UART position and Power switch in USB position).

![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/LinkIt_ONE_Wiki_Temp3.jpg) 
- Open **File** -> **Examples** -> **Basics** -> **Blink** in LinkIt ONE IDE.
- Select the COM Port number corresponding to **MTK USB Debug port** in **Tools** -> **Port**.
- Compile and upload the code.
- LED marked **L** should blink.

### Connecting Antennae
There are three antennae provided with LinkIt ONE. They are used for:
- GSM/GPRS
- Wi-Fi/BT
- GPS

Connect the antenna as the following image.

![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/400px-Linkit_one_antenna.jpg) 

**Note:**
- While pulling the antenna from board, do it with care. Please Do not use brute force.
- Try to use the force perpendicular to the direction of the board, otherwise you might damage the antenna pad.

### Inserting SIM Card and SD Card

LinkIt ONE accepts standard size SIM Card and Micro SD Card. Insert them as per the following image:

![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/LinkItONE_SIM_SDCard_Insert.jpg) 

### Exploring LinkIt ONE SDK Examples
LinkIt ONE SDK comes with many examples / sample code to use peripherals like GSM, GPRS, WiFi, BT, Audio, GPS etc. Explore them first and read about API documentation. API documentation are available in [  User Guide ](http://labs.mediatek.com/fileMedia/download/5fed7907-b2ba-4000-bcb2-016a332a49fd) and [  API References site ](https://labs.mediatek.com/site/znch/developer_tools/mediatek_linkit/api_references/Core_Digital.gsp)


## Compatible Groves and Shields for LinkIt ONE

- We manufacture hundreds of Groves and Shields, including sensors, actuators, displays and other modules.
- You can implement your ideas with those Groves and Shields easily.
- But, LinkIt ONE does not support all of them.
- We prepared a list of compatible Groves and Shields:

[![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/400px-Compatible_Groves_and_Shields_for_LinkIt_ONE.png)](https://github.com/SeeedDocument/Linkit-ONE/blob/master/resource/LinkIt_ONE_Comparability_Test.xlsx)

## Tutorial of Sidekick Basic Kit for LinkIt ONE

The Sidekick Basic Kit for LinkIt ONE is designed to be used with your LinkIt ONE board. This kit will help you quickly get along well with the platform of LinkIt. It includes many of the most popular accessories for DIY projects : like Breadboard, Jumper wires, Color LEDs, Resistors, Buzzer, etc. All these come in a handy box, which is easy to transport and mimimises clutter. The kit includes a complete guide that will familiarize you with a wide range of electronic components while you create small, simple, and easy-to-assemble circuits. There are 10 different courses outlined that will offer a best way for beginner to get familiar with LinkIt ONE.

**SKU:**[110060038](https://www.seeedstudio.com/item_detail.html?p_id=2027)
- [The Basics](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_The_Basics)
- [Hello World](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_Hello_World)
- [Push Button](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_Push_Button)
- [Marquee](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_Marquee)
- [Colorful World](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_Colorful_World)
- [Analog Interface](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_Analog_Interface)
- [Mini Servo](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_Mini_Servo)
- [Light Sensor](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_Light_Sensor)
- [SMS Control the LED](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_SMS_control_the_LED)
- [Get Temperature with Webpage](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_Get_temperature_with_Webpage)

- [Github Repo for Sidekick Basic Kit for LinkIt ONE](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_Get_temperature_with_Webpage)


## Related Projects

If you want to make some awesome projects by LinkIt ONE, here's some projects for reference.

### Make an Instructables Indicator
[Instructables](http://www.instructables.com/)is really an awesome place to share your awesome project. There’s so many makers here to share their works.
I had made many instructable as well, I will feel excite when my instructable get a large views or favorites. Especially when you first post your instructable, you will always go to the page and see if someone like it.
I still remember when I post my first instructable years ago, it’s a project about Arduino, I made a phone with Arduino. It’s called [ArduinoPhone](http://www.instructables.com/id/Make-a-Instructables-Indicator/)even today I can get some comments from it, and I am glad to help others to make their own phone with Arduino.

Now, I will share my latest instructable, it’s a beautiful device that you can put it on the desk. It’s named Instructables Indicator. With this instructable, you can know if people like your instructable, if your instructable get featured.

This application contains the below function:

Connecting to Wi-Fi

- A 320x240 TFT display to show the message
- Include Views, Favorites and Comments.
- When your instructable get featured, the leds on the base will turn on

If you like Instructables and write instructables, you will like this idea. I will share the process to make it, as well as the code, all things is open sources.

[![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/200px-Wiki_makeitnow_logo.png)](http://www.instructables.com/id/Make-a-Instructables-Indicator/)

### Acrylic Case
If you need a acrylic case to protect your LinkIt ONE.

There's a tutorial to help you to make one.

[![](https://raw.githubusercontent.com/SeeedDocument/Linkit-ONE/master/image/200px-Wiki_makeitnow_logo.png)](http://www.instructables.com/id/5-Design-of-Laser-Cut-Cases-for-5-Popular-Platform/)

### Other projects about LinkIt ONE

- [Awesome Projects at Recipe](http://www.seeed.cc/discover.html?t=linkit)
- [Awesome Projects at Instructables](http://www.instructables.com/id/Mediatek-LinkIt-ONE/)

## Resources
Schematic / Design Files:
- [LinkIt ONE V1.0 Eagle File](http://www.seeedstudio.com/wiki/LinkIt_ONE_Tutorial_-_The_Basics)

Software:
- [MediaTek_LinkIt_SDK_for_Ardunio](http://labs.mediatek.com/site/znch/developer_tools/mediatek_linkit/sdk_intro/index.gsp)

Datasheets and User Guides:
- [LinkIt_ONE_Hardware_Reference_Design_v1_0](http://labs.mediatek.com/site/znch/access_denied/access_denied.gsp)
- [LinkIt ONE_Pinout Diagram_v1.0【PDF】](https://github.com/SeeedDocument/Linkit-ONE/blob/master/resource/LinkIt_ONE_Pinout_Diagram_v1_0.pdf)
- [MediaTek_LinkIt_Developers_Guide_v1_0【PDF】](https://github.com/SeeedDocument/Linkit-ONE/blob/master/resource/MediaTek_LinkIt_ONE_Developers_Guide_v1_3.pdf)
- [MediaTek_MT2502A_SOC_Data_Sheet_v1_0【PDF】](https://github.com/SeeedDocument/Linkit-ONE/blob/master/resource/MediaTek_MT2502A_SOC_Data_Sheet_v1_0.pdf)
- [MediaTek_MT5931_Wi-Fi_Data_Sheet_v1_0【PDF】](https://github.com/SeeedDocument/Linkit-ONE/blob/master/resource/MediaTek_MT5931_Wi-Fi_Data_Sheet_v1_0.pdf)
- [MediaTek_MT3332_GPS_Data_Sheet_v1_0【PDF】](https://github.com/SeeedDocument/Linkit-ONE/blob/master/resource/MediaTek_MT3332_GPS_Data_Sheet_v1_0.pdf)

Getting Help
- [Seeedstudio LinkIt ONE Forum](http://www.seeed.cc/discover.html?t=linkit)
- [MediaTek LinkIt ONE Forums](https://labs.mediatek.com/forums/forums/list.page)

More
- [See Also: Sidekick Base Kit for LinkIt ONE](http://www.seeedstudio.com/wiki/Sidekick_Basic_Kit_for_LinkIt_ONE)






