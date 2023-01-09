# QNBPMachineDevice

血压计设备

#### 成员变量

| 名称     | 类型   | 描述         |
| -------- | ------ | ------------ |
| bleName  | String | 蓝牙名       |
| mac      | String | mac地址      |
| modelId  | String | 设备类型标识 |
| rssi     | int    | 信号强度     |
| protVer | int    |  协议版本     |
| hemVer | int    |  血压计版本     |
| bleVer   | int    | 蓝牙版本     |

### getSupportWiFi

获取设备是否支持WiFi功能

##### 参数
   无

##### 返回值
| 类型 | 描述 |
| ------ | ------ |
| Bool | 是否支持WiFi功能 |


### getSupportChangeLanguage

获取设备是否支持语言切换功能(需在设备允许交互后调用有效)

##### 参数
   无

##### 返回值
| 类型 | 描述 |
| ------ | ------ |
| Bool | 是否支持语言切换功能 |

### getSupportChargeBattery

获取设备是否支持充电功能(需在设备允许交互后调用有效)

##### 参数
   无

##### 返回值
| 类型 | 描述 |
| ------ | ------ |
| Bool | 是否支持充电功能 |


### getCurrentLanguage

获取设备当前语言类型(需在设备允许交互后调用有效)

##### 参数
   无

##### 返回值
| 类型 | 描述 |
| ------ | ------ |
| [QNBPMachineLanguage](./QNBPMachineDeploy.md#qnBPMachinelanguage) | 语言 |


### getCurrentUnit

获取设备当前单位类型(需在设备允许交互后调用有效)

##### 参数
   无

##### 返回值
| 类型 | 描述 |
| ------ | ------ |
| [QNBPMachineUnit](./QNBPMachineDeploy.md#qnBPMachineunit)  | 单位      |


### getCurrentStandard

获取设备当前血压标准类型(需在设备允许交互后调用有效)

##### 参数
   无

##### 返回值
| 类型 | 描述 |
| ------ | ------ |
| [QNBPMachineStandard](./QNBPMachineDeploy.md#qnBPMachinestandard)  | 血压标准      |
