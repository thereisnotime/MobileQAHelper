# MobilaQAHelper

### Description ###
Simple GUI for scrcpy to help QA engineers control multiple different mobile devices from their Windows.

* NOTICE: This is still a WIP. Few bugs need to be fixed before I upload the code.

### Features ###
- Open interactive session to every connected Android device 
- View physical screen touches on the computer session of the device
- Open a session with physical screen turned off
- Open a read-only session
- Record a session to video file
- View if Android device is being used by another user on this computer
- Open a session with FPS counter

### Screenshots ###
![Screenshot1](/Screenshots/Screenshot_1.png?raw=true "Main WIP window.")

### Installation ###
No installation is needed, download the release or build it yourself from source.

### Dependencies ###
Required .NET framework:
```sh
Microsoft .NET Framework 4.6.1
````
Required libraries:
```sh
LibUsbDotNet.dll
MaterialSkin.dll
SharpAdbclient.dll
````
Required software:
```sh
adb + drivers
scrcpy
````

### Compatability ###
The should work on most Windows versions and has been tested on the following:
```sh
Windows 10 Home x64
Windows 10 Professional x64
Windows Server 2019
Windows Server 2016
``` 

### Notes ###
Most of the functions depend on finding a window by its caption (device model + device serial number). If you change the session window title hell will rain down upon you.

### Todo ###
Add ability to send keystrokes to SDL handles (for shortcut buttons).
Move logging to separate thread.
Move all functions to separate thread so UI remains responsive.
Add a downloader for scrcpy.
Add a check if generic (adb)Android USB drivers are installed.
Add Wi-Fi ability and arp listener for new devices.
Add local file database for previous connected devices.
Check if adb is installed and running.
Add stdout/err capture of each new window handle.
Add better process event handling.
Add thumbnail preview of already opened sessions.
Add ability to clone window for read-only purposes.

### Uninstall ###
Delete the executable.

