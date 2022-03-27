ets2_dashboard
==============

**Euro Truck Simulator 2 Arduino Dashboard Code**

This is the code for my dashboard project, there is a
[blog post](http://skyhisi.blogspot.co.uk/2013/09/euro-truck-simulator-2-prototype-real.html)
which contains photos and videos of it working and how it works.

Installing
----------

1.  Connect up some servos and LEDs to your Arduino
2.  Change the pin assignment in the `arduino_controller.ino` file and flash to the Arduino
3.  Copy a pre-built DLL into your ETS2 plugins folder
    *or*
4.  Build the DLL by running the `build.bat` file from a Visual Studio 2010 command prompt
5.  Copy the `dash_plugin.txt` options file into the plugins folder

Troubleshooting
---------------

- Check you have copied the `dash_plugin.txt` file as well as the DLL into the plugins folder
 
- Check the Arduino is on COM3 - the plugin expects to find the Arduino on COM3, you can change this by editing the `dash_plugin.txt` options file

- Check for error messages in the game log (in `%USERPROFILE%\Documents\Euro Truck Simulator 2\game.log.txt`).  

Setup Development Environment
---------------

This fork was set up to use Visual Studio Code. Complete the following steps to setup your local development environment.

1. Download and install Visual Studio Code (https://code.visualstudio.com)
2. Install the **Desktop development with C++** workload of the **Visual Studio Build Tools** (https://visualstudio.microsoft.com/downloads#other)
3. Install Git (for example on Windows 10: `winget install Git.Git`)
4. Clone the repository and open in Visual Studio Code
5. Download the latest SCS Telemetry SDK (https://modding.scssoft.com/wiki/Documentation/Engine/SDK/Telemetry)
6. Extract the SDK into the local SDK folder of the repository
7. Optionally install the Arduino IDE ((for example on Windows 10: `winget install Arduino`))

You're all set!