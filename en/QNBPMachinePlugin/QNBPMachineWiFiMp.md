# QNBPMachineWiFiMp
血压计设备WiFi管理

## API

### setWiFiStatusListener
设置设备WiFi监听器

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| wifiListener | [QNBPMachineWiFiListener](./QNBPMachineWiFiListener.md) | 设备WiFi监听器 |


### startConnectWiFi

开始配置设备WiFi

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device  |  [QNBPMachineDevice](./QNBPMachineDevice.md)   | 血压计设备 |
| wifiInfo  | [QNBPMachineWiFi](./QNBPMachineWiFi.md)  | WiFi信息 |

##### 返回值
类型：[int 详情见状态码列表](../Code.md#wifi相关)

### scanNearbyWiFi

扫描附近WiFi

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device  |  [QNBPMachineDevice](./QNBPMachineDevice.md)   | 血压计设备 |

##### 返回值
类型：[int 详情见状态码列表](../Code.md#wifi相关)

