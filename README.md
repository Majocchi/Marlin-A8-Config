# Marlin-ANET-Config ( A6 / A8 ) 2021

It's a bit tricky to get Marlin v 2.08 (Release 30. April 2021) compiled for ANET A8 3d-Printer on Windows 10.

Here's what you need to get it work:

# SkyNet3D v 2.4.5 / MARLIN 1.1.x

1.) modified Arduino IDE Version 1.8.10 [ https://github.com/Majocchi/Marlin-ANET-Config/releases/tag/1.0 ]

    -> https://github.com/Majocchi/Marlin-ANET-Config/releases/download/1.0/anet-arduino-1810.zip

2.) modified Marlin Version 1.1.9.1 [ https://github.com/Majocchi/Marlin-ANET-Config/releases/tag/1.05 ]

    -> https://github.com/Majocchi/Marlin-ANET-Config/releases/download/1.05/Marlin-1191.zip

3.) Windows USB to Serial driver for ANET 1.x Board [ https://github.com/Majocchi/Marlin-ANET-Config/releases/tag/0.9 ]
   
    -> https://github.com/Majocchi/Marlin-ANET-Config/releases/download/0.9/CH340drv.zip

# Let's GO !

- Unzip Arduino to a short Path ( like c:\arduino )
- Unzip Marlin to your Ardunio path -> ..\portable\sketchbook\Marlin
- Install Windows USB Serial Driver & connect your ANET v1.x Board (powered by 12V)
- Open arduino.exe and set your serial port -> Tools / Port / COMx
- Your Board needs a Arduino Bootloader; if not already done, flash it with USBasp ( Tools / Programmer / Usbasp > Burn bootloader )
 
   -> Descriptions how to to do this can be found on Youtube and Google, e.g.:
      https://www.youtube.com/watch?v=3jm0zzIneFc
      https://chriss.gebbing.de/3d-drucker/anet-board-1-7-mit-bootloader-flashen/
      https://01001000.xyz/2020-08-06-Updating-Firmware-Anet-A8-Board-1.7/
      
- Choose the config.h file which meets your Printer best [ https://github.com/Majocchi/Marlin-ANET-Config/releases/tag/1.2 ]

  and copy it to ..\portable\sketchbook\Marlin\Configuration.h
  
  ...adapt to your needs if necessary, take a look @ https://marlinfw.org/docs/configuration/configuration.html#configuring-marlin

- Click Upload - Congratulations >> MARLIN is READY for YOU !!!


# MARLIN v 2.0.x

This is much easier :-)

1.) Install Windows USB Serial Driver & connect your ANET v1.x Board (powered by 12V) https://github.com/Majocchi/Marlin-ANET-Config/releases/tag/0.9

2.) Install VScode https://code.visualstudio.com

3.) Install PlatformIO IDE for VScode  https://platformio.org/platformio-ide

4.) Install "Auto Build Marlin" for VScode https://marketplace.visualstudio.com/items?itemName=MarlinFirmware.auto-build

5.) Download & Unzip latest Marlin v 2.0.x Version  https://github.com/MarlinFirmware/Marlin/releases

6.) Choose the config.h file which meets your Printer best [ https://github.com/Majocchi/Marlin-ANET-Config/releases/tag/1.2 ]

and copy it to the unzipped Marlin folder ..\Marlin}Configuration.h 

- Click Compile % Upload in "Auto Build Marlin" - Congratulations >> MARLIN is READY for YOU !!!

( Here you can find a YouTube Video about it https://www.youtube.com/watch?v=d_GfpI90uo8 )




If you like the Marlin Firmware - please donate for it @ https://www.thinkyhead.com/donate-to-marlin or

# if my work helped you, think about buying me a coffee :-)

https://paypal.me/Majocchi

XMR: 4B1CmUg5LGUgozGPbSTochbiXfqEcNVbtN7svHywi5iiMHeEK2Gwwqc72uasfWpeUgZ1otyaqWjhYZUrHg3Xv8NZSwP9DHX

(segwit) BTC:  3GLkVdTNXeKusit1j8yvdzMS75XrfzrEiP

(native) BTC:  bc1q5hxhrdhpvuefs30jx7gr7rccex8t7kh5lx23f5

   ETH:  0xDC2251AC130aB3bCb07E703cedA02e2af9Cc1925


