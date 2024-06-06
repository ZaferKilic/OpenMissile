
<p align="center">
  <img src="https://github.com/ZaferKilic/OpenMissile/blob/main/Gallery/Logo.png?raw=true" />
</p>

## Table of Contents

1. [Features](#features)
2. [Introduction](#introduction)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Examples](#examples)
6. [License](#license)

## Features
- Visualize flight data
- 3D simulation
- Instant location tracking
- Voice alerts
- Sending command or data to the rocket
- Distance calculation between ground station and rocket
- Data rate measurement
- Estimated drop point in case of data loss
- Video stream
- Sharing flight data via TCP
- Compliant with Teknofest competition standards
- Record flight data



## Introduction
<span style="color: #000; font-family: Museo Sans Cyrl; font-size: 1em;">OpenMissile is a ground station software developed for visualizing data from the RF module of model rockets and performing various calculations.</span>
![alt text](https://github.com/ZaferKilic/OpenMissile/blob/main/Gallery/ScreenShot2.png?raw=true)



## Installation
```
pip3 install -r requirements.txt
```

## Usage
OpenMissile uses the JSON format to parse data coming from the serial port. It writes the data into the appropriate Labels using unique keys for each piece of data.
If you are using an Arduino-based microcontroller, you can use the <a href="https://github.com/bblanchon/ArduinoJson">ArduinoJson</a> library.

## Examples

- Incoming serial port data
```
    {
        "SeaAlt": 123.00,
        "X": 36.01,
        "Y": 76.01,
        "Z": 2.01,
        "Apogee": 1500
    }
```



## License
This project is licensed under the MIT License. For more details, see the LICENSE file.
