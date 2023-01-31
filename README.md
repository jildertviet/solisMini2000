# solisMini2000
ESPHome modbus application for Home Assistant integration for the Solis Mini 2000 4G solar inverter

## Hardware  
- ESP32 (I use a Wemos Lolin D32)
- MAX485 board (I've desoldered the connector and soldered the wires directly)
- 4-pin connector (harvested from the original dongle)

Connect 
| ESP32        | MAX485    |
|--------------|-----------|
| 16           | RO        |
| 17           | DI        |
| 4            | DE & RE   |
| 3.3V         | VCC       |
| GND          | GND       |

| ESP32        | connector |
|--------------|-----------|
| USB          | Red       |
| GND          | Black     |

| MAX485       | connector |
|--------------|-----------|
| A            | Yellow    |
| B            | Blue      |

## Secrets
- Create secrets.yaml file with:
```
ssid: "xxx"
password: "xxx"
fallbackpassword: "xxx"
myPw: "xxx"
```
And replace _xxx_ with your data
