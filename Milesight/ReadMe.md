# LORA to modbus TCP
## Instructions
- Set the device UIDs in the switch block.
- Set the modbus address in the "UNIT" Environment Vaiable in the subflow

## Modbus Addresses
### AM103+L
| Mobus address | Type | Function |
|--|--|--|
| 1 | Holding | Battery * 10 (%) |
| 2 | Holding | CO2 (ppm) |
| 3 | Holding | Humidity * 10 (%RH) |
| 4 | Holding | Temperature * 10 (°C) |
| 5 | Holding | RSSI * -1 (dBmW)
| 6 | Holdnig | ( SNR + 100 ) * 10 |
| 7 | Holding | 0 = OK, 1 = fault (5 hours since last packet) |
| 8 | Holding | Spread Factor |
