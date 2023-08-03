# Node Red flow for modbusTCP integration with any modbusTPC BMS system
## instructions
### Node red
set the appripriate invironment variables on the subflows.

### Modbus
#### main device

|  address |  type |  function |
| ------------ | ------------ | ------------ |
|  1 | coil  |  hearbeat from SCnordic (false if problem) |
|  2 |  input |  heartbeat to SC nordic (expects a changing, random, non-zero number) |
|  3 |  coil |  Command from SC nordic (true is control, false is auto) |
|  4 |  coil |  return status of "3" to SC nordic |

