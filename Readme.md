<p align="center">
  <img width="150" height="150" src="https://github.com/IPI-Patrick/turtle-tough-app-release/blob/main/icon.png">
</p>

<h1 align="center">
    <b> Turtle Tough Sensor Management Software </b>
</h1>

The Turtle Tough Smart Sensor PC Interface (TT-ACC-DSS-WIB) provides an easy plug & play PC interface for all our Smart Sensors.  It is one of the most comprehensive tools you can have for complete sensor communications and diagnostics. The interface provides a USB to RS485 interface for the smart sensors as well as providing power to the sensor via the USB power supply.   Connecting your Smart Sensors to a PC allows you to use our Windows PC Communication and Configuration Software as well as connect to 3rd party applicaitons for programming or control purposes.

The Turtle Tough Windows PC Software provides a powerful tool for communication and configuration.  The software enables you to view the sensor readings in real time, which is ideal for lab or benchtop based work without the need for a benchtop meter or analyser. You also have complete access to sensor diagnostics and critical sensor information for determining sensor health and lifetime. A central part of the software allows you to perform calibrations as well as print calibration reports.

Designed for industrial environments, the Smart Sensor PC Interface is housed in a rugged NEMA 4X enclosure and features 3x NEMA 6P quick connect plugs for simultaneous connection of up to 3 Smart Sensors.  This device is a must have for anyone running Turtle Tough Smart Sensor technology.



# Installation:
To Install This software, simply download the latest release from [Releases](https://github.com/IPI-Patrick/turtle-tough-app-release/releases/tag/v0.1.19) and run the executable.

***Note:*** *On windows a Windows Defender Smartscreen window may appear. If so, simply click "More Info" then "Run Anyway". This is simply an artifact of the digital signing process and will be fixed shortly.*

# Basic Usage - Connecting Sensors:
To connect a sensor to the software, start by opening the software and connecting your Turtle Tough Smart Sensor Communication Hub to your PC via the USB cable, in any order. The software should automatically identify and connect to your Communication Hub.

Next, connect your Turtle Tough Digital Smart Sensor to the Communication Hub. Your sensor may appear automatically. If it does not, scan for the sensor by pressing the "Scan For Sensors" button in the sidebar. This will scan for all connected sensors on the modbus network. When your sensor has been located it will appear automatically in the dashboard. At this point you can click "Finish Scan" and begin using your sensor.

# Basic Usage - Calibration:
Calibration using the Turtle Tough Sensor Management software is easy. Once your sensor is connected, open its information page by clicking on the sensor in either the dashboard or the sidebar.

The calibration panel will be shown in the sensors information page near the top. Start by choosing your calibration type (3 Point, 2 Point, etc) and enter the values of your buffer solutions.

  *Please note that if "Use Default Buffers" is selected then the values will automatically adjust to the ones set in the application settings menu. To change these values click on the settings button in the sidebar and enter your default buffer values.*

Click 'Begin Calibration' to start calibrating. To calibrate any point simply place the sensor in the correct buffer and wait till the Sensor Readings Widget shows that your sensors readings are stable. Once your sensor is stable click 'Calibrate ***' to calibrate. Repeat for all calibrations. 

Once the calibration is complete your calibration results will be displayed in the 'Print' panel. Click the 'Print Calibration Report' Button to print a report.


# Roadmap
- ## First Official Release
    - **Live Readings;** Ability to get and display live readings of multiple connected digital Turtle Tough pH sensors on a beautiful, easy to read dashboard.
    - Basic plotting of live sensor readings for easy diagnostics.
    - **Easy Connection;** Automatic connection to Turtle Tough Smart Sensor Communication Hub's with fast re-connection of previously connected Turtle Tough Sensors.
    - **Sensor Scanning;** Easily scan for newly connected sensors with unknown modbus addresses.
    - **Sensor Configuration;** Ability to configure sensors with their own unique name for easy identification.
    - Allows all sensor settings to be configured directly from the application.
    - **Sensor Calibration and Diagnostics;** Simple calibration of all Digital pH sensors with the ability to print calibration reports and remember the results of the last calibration. 
    - Sensor health score generated via a set of complex heuristics from the last completed calibration. 

- ## Version 1.x
  - Support for further Turtle Tough Digital Sensor Types.
  - Support for digital ORP, Conductivity and Dissolved Oxygen Sensors.
  - Add support for Mac and Linux operating systems.
  - Add support for multiple languages.

- ## Version 2.0 (Lab Version)
  - **Plotting Overhaul;** Allow for extensive real-time plotting options, allowing readings to be taken, displayed, saved and exported at the users discretion.
  -  **Syncing Between computers;** Ability for multiple computers to be running the software simultaneously, sharing sensor readings, information and control between them. 
  - **Rich Diagnostic History;** Allow storing of much more in depth sensor diagnostic history including calibration results and overall lifespan. 
  - **Reminders and Warnings;** Send reminders to calibrate sensors at certain intervals or create triggers to send warnings when sensor readings reach certain thresholds.


# Troubleshooting:

### My Communication Hub is Not Connecting ##
- Older Turtle Tough Smart Sensor Communication Hubs may not have the correct digital signature to be automatically recognised by the software. If this is the case a manual connection can be made to the hub by clicking the "Device Not Appearing Automatically" button. In this menu, select the COM Port that your device is connected to and the correct Modbus settings (by default baud-rate is 19200 and parity is 'Even') then click "Connect". If the settings are correct then you should now be connected to the Communication Hub.

### My Sensor is Not Appearing ##
- If your sensor is not appearing automatically when connected then this may mean it has a different node address to what the software is looking for. To find your sensor, click the 'Scan For Sensors' button in the sidebar. The software will begin scanning for sensors on the Modbus network. Once all your sensors have been identified, click the 'Finish Scan' button to complete the scan. If you sensor is not found during this scan, try disabling the 'Quick Scan' feature by pressing the up arrow and toggling the 'Quick Scan' switch, then restarting the scan.

### My Sensor Dissapears When I Connect Another Sensor ###
- If your sensor dissapears when another sensor is connected then the most likely cause is that the two sensors are both using the same Modbus node address. If this is the case then the address of one sensor must be changed. To do this, connect one of the sensors and leave the other disconnected. Navigate to the sensors information page by clicking on the sensor and scroll down to the 'Sensor Settings' section. In this section identify the 'Node' setting and change this to be a different number between 0 and 255.
  
  
# Support & Feature Request:
If you have any questions about the application or have found any issues or bugs, please email Turtle Tough at support@industrialsensors.com.au and we will endeavour to get back to you as soon as we can.