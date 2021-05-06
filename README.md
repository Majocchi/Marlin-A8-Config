# Marlin-ANET-Config ( A6 / A8 ) 2021

It's a bit tricky to get Marlin v 2.08 (Release 30. April 2021) compiled for ANET A8 3d-Printer on Windows 10.

Here's what you need to get it work:

1.) modified Arduino IDE Version 1.8.10 [ https://github.com/Majocchi/Marlin-ANET-Config/releases/tag/1.0 ]

    -> https://github.com/Majocchi/Marlin-ANET-Config/releases/download/1.0/anet-arduino-1810.zip

2.) modified Marlin Version 2.0.8 [ https://github.com/Majocchi/Marlin-ANET-Config/releases/tag/1.1 ]

    -> https://github.com/Majocchi/Marlin-ANET-Config/releases/download/1.1/Marlin.zip

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


If you like the Marlin Firmware - please donate for it @ https://www.thinkyhead.com/donate-to-marlin

or 

# if my work helped you, think about buying me a coffee :-)

https://paypal.me/Majocchi

XMR: 4B1CmUg5LGUgozGPbSTochbiXfqEcNVbtN7svHywi5iiMHeEK2Gwwqc72uasfWpeUgZ1otyaqWjhYZUrHg3Xv8NZSwP9DHX

BTC: 3EFW7SLZ8ee7xJ3m7Hk9aCE65Q9voSrDEs

ETH: 0xbd7c116f064d2d141bba28da49644b501c7d5cec
