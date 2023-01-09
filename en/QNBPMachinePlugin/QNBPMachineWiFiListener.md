# QNBPMachineWiFiListener
设备WiFi监听器，用于监听回调设备配置WiFi状态

## API

### onDiscoveryNearbyWiFi
发现附近WiFi

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| ssid |   String   | WiFi名称 |
| rssi |   Int   | WiFi信号强度 |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |


### onStartWiFiConnect
开始为血压计配置WiFi

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |

### onConnectWiFiStatus
血压计配置WiFi结果

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| code       | [int 详情见状态码列表](../../Code.md#wifi相关)  | 状态码 |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |