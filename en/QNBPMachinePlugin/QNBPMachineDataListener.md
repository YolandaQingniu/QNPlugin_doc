# QNBPMachineDataListener

设备数据监听器，用于监听回调设备测量数据；

## API

### onReceiveRealTimeData
血压计实时测量完成结果数据回调

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| measureResult            | [QNBPMachineMeasureResult](./QNBPMachineDataListener.md#qnbpmachinemeasureresult)  | 本次测量结果状态 |
| data            | [QNBPMachineData](./QNBPMachineData.md)  | 测量数据结果, 当测量失败是 data为nil |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |

### onReceiveStoredData
血压计收到存储数据列表回调

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| data            | [QNBPMachineData](./QNBPMachineData.md)  | 存储数据结果 |
| device | [QNBPMachineDevice](./QNBPMachineDevice.md) | 血压计设备 |


#### QNBPMachineMeasureResult
|名称  | 含义   |
| ------ |------|
|QNBPMachineMeasureResultUndone | 未测量完成  |
|QNBPMachineMeasureResultErr1 | 设备未标定 |
|QNBPMachineMeasureResultErr2 | 袖带脱离/动作过大  |
|QNBPMachineMeasureResultErr3 | 高压检测失败 |
|QNBPMachineMeasureResultErr4 | 低压检测失败  |
|QNBPMachineMeasureResultErr5 | 未检测到血压脉动  |
|QNBPMachineMeasureResultErr6  | 测量超时 |
|QNBPMachineMeasureResultErr7  | 过度加压   |
|QNBPMachineMeasureResultErr8  | 加压过程中出现漏气 |
|QNBPMachineMeasureResultErr9  | 未连接袖带 |
|QNBPMachineMeasureResultSuccess  | 测量成果   |
