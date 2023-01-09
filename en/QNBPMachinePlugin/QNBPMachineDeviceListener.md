# QNBPMachineDeviceListener

设备相关事件监听器

## API

### onDiscoverBPMachineDevice

搜索到血压计设备的事件回调

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |


### onBPMachineConnectedSuccess
血压计设备连接成功

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |

### onBPMachineConnectFail
血压计设备连接失败

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| code   | [int 详情见状态码列表](../Code.md#设备相关)    | 状态码     |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |

### onBPMachineReadyInteractResult
血压计设备准备完成,可以开始设置交互

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| code   | [int 详情见状态码列表](../Code.md#设备相关)    | 状态码     |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |


### onSetBPMachineFunctionResult

设置血压计设备功能结果

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| code   | [int 详情见状态码列表](../Code.md#设备相关)    | 状态码     |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |

### onBPMachineDisconnected
血压计设备断开连接

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |