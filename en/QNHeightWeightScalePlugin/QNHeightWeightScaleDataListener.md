# QNHeightWeightScaleDataListener
设备数据监听器，用于监听回调设备测量数据；

## API

### onHeightWeightScaleRealTimeWeight
设备实时体重回调

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| weight            | String                   | 体重，单位kg |
| device |   [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |

### onHeightWeightScaleRealTimeHeight
设备实时身高回调

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| height            | String                   | 身高，单位cm |
| device  |  [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |

### onHeightWeightScaleReceiveMeasureResult
设备测量完成结果数据回调

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| scaleData   | [QNHeightWeightScaleData](./QNHeightWeightScaleData.md) | 测量数据 |
| device  |  [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |

### onHeightWeightScaleReceiveMeasureFailed
测量失败

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device |    [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |

### onHeightWeightScaleReceiveStorageData
设备收到存储数据列表回调

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| list   | [[QNHeightWeightScaleData](./QNHeightWeightScaleData.md)] | 存储数据列表 |
| device  |  [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |
