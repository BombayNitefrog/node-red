# Node Red flow for modbusTCP integration with any modbusTPC BMS system
## instructions
import flow into node-red

set the topics and copy devices to match actual topics and number of devices.

### Modbus
#### main device
x = device number

| deviceAddress |  address |  type |  function |
| --- | ------------ | ------------ | ------------ |
| 100 |  1 | coil  |  hearbeat from SCnordic (false if problem) |
| 100 |  2 |  input |  heartbeat to SC nordic (expects a changing, random, non-zero number) |
| 101 |  x0 |  coil |  Command from SC nordic (true is control, false is auto) |
| 101 |  x1 |  coil |  return actual activation status of device |
| 101 |  x2 |  int |  Step Command for device |
| 101 | x3 | int  | return actual step status of device |

