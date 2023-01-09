# QNBPMachinePlugin

血压计设备管理

## API

### setBPMachinePlugin

设置血压计管理类

##### 参数

| 名称   | 类型                                | 说明       |
| :----- | :---------------------------------- | :--------- |
| plugin | [QNPlugin](../QNPlugin/QNPlugin.md) | 基础管理类 |

##### 返回值

类型：[int 详情见状态码列表](../Code.md#初始化相关)

### setDeviceListener

设置设备监听器

##### 参数

| 名称           | 类型                                                         | 说明           |
| :------------- | :----------------------------------------------------------- | :------------- |
| deviceListener | [QNBPMachineDeviceListener](./QNBPMachineDeviceListener.md) | 设置设备监听器 |

### setDataListener

设置设备数据监听器

##### 参数

| 名称         | 类型                                                         | 说明           |
| :----------- | :----------------------------------------------------------- | :------------- |
| dataListener | [QNBPMachineDataListener](./QNBPMachineDataListener.md) | 设置数据监听器 |

### connectDevice

连接设备

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |

##### 返回值

类型：[int 详情见状态码列表](../Code.md#设备相关)

### cancelConnectDevice

断开设备连接

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |

### setDeviceFunction

设置设备功能

##### 参数

| 名称   | 类型                                                          | 说明       |
| :----- | :----------------------------------------------------------- | :--------- |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md)            | 血压计设备   |
| deploy | [QNBPMachineDeploy](./QNBPMachineDeploy.md)            | 功能配置项   |

##### 返回值

类型：[int 详情见状态码列表](../Code.md#设备相关)

### readStoredData

读取存储数据

##### 参数

| 名称   | 类型                                                          | 说明       |
| :----- | :----------------------------------------------------------- | :--------- |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md)            | 血压计设备   |

##### 返回值

类型：[int 详情见状态码列表](../Code.md#设备相关)

