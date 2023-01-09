# QNHeightWeightScaleDeviceListener
设备相关事件监听器

## API

### onDiscoverHeightWeightScaleDevice
搜索到设备的事件回调

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device  | [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md) | 身高一体机设备 |


### onSetHeightWeightScaleUnitResult
设置秤端单位结果回调

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| code       | [int 详情见状态码列表](../Code.md#设备相关)                   | 状态码 |
| device   | [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |


### onHeightWeightScaleConnectedSuccess
设备连接成功回调
##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device   | [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |

### onHeightWeightScaleConnectFail
设备连接失败

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device   | [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |

### onHeightWeightScaleReadyInteract
设备已准备完成，可以开始交互

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| code       | [int 详情见状态码列表](../Code.md#设备相关)                  | 状态码 |
| device   | [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md) | 身高一体机设备 |

### onHeightWeightScaleDisconnected
设备已断开连接
##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device    |[QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |
