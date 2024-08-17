<p align="center">
  <img src="https://github.com/ZaferKilic/OpenMissile/blob/main/Gallery/LargeLogoBG.png?raw=true" />
</p>

<span> A ground station that visualizes and processes real-time data obtained from model rockets.
<br>
<br>
I will not be releasing the project's code for now. I will only provide it as a 1-month trial version to interested teams. Perhaps in the coming weeks, if I feel the project is complete in my mind, I might offer the full version for sale at a reasonable price.</span>

![alt text](https://github.com/ZaferKilic/OpenMissile/blob/main/Gallery/RocketPage.png?raw=true)

## Features
- Data Visualization
- 3D Simulation
- Real-time location tracking on the map  
- Audible Alerts
- Sending commands to the rocket
- Distance calculation between the rocket and ground station
- Data transmission rate measurement
- [BETA] Landing point estimation in case of data loss
- Viewing camera footage from the rocket
- Sending data to a remote server via TCP
- Developed according to Teknofest Rocket Competition standards
- Sending data from the ground station to Teknofest judges
- Flight data recording
- Customizable interface

## Usage
OpenMissile uses the JSON format to parse data coming from the serial port. It writes the data to appropriate Tags using unique keys for each data piece.
If you are using an Arduino-based microcontroller, you can use the following library: <a href="https://github.com/bblanchon/ArduinoJson">ArduinoJson</a>. 

The faster the data can be received, the smoother the 3D simulation will run. However, for teams using RF modules that are not suitable for fast data transmission, it is recommended to send data to OpenMissile every 5 received data.

## Examples
- If you hover over the sections where data is written within OpenMissile, you can see which key it uses.
- Example of accepted data:

```
    {
    "SeaAlt": 123.00,
    "vSpeed": 123.00,
    "Temp": 123.00,
    "Pressure": 123.00,
    "X": 36.01,
    "Y": 76.01,
    "Z": 2.01,
    "AccX": 36.01,
    "AccY": 36.01,
    "AccZ": 36.01,
    "GForce": 36.01,
    "Apogee": 1500,
    "Latitude": 39.9250533,
    "Longitude": 32.8361282,
    "GpsAlt": 36.01,
}
```



## Lisans
This project is licensed under the MIT License. For more details, see the LICENSE file.
