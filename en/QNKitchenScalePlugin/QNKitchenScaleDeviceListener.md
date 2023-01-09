# QNKitchenScaleDeviceListener

设备相关事件监听器

## API

### onDiscoverKitchenScaleDevice

搜索到设备的事件回调

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |

### onSetKitchenScaleUnitResult

设置单位结果

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| code   | [int 详情见状态码列表](../../Code.md#设备相关)    | 状态码     |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |

### onSetKitchenScaleShellingResult

设置去皮结果

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| code   | [int 详情见状态码列表](../../Code.md#设备相关)    | 状态码     |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |

### onSetKitchenScaleStandTimeResult

设置设备亮屏时间

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| code   | [int 详情见状态码列表](../../Code.md#设备相关)    | 状态码     |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |

### onKitchenScaleConnectedSuccess

设备连接成功回调

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |

### onKitchenScaleConnectFail

设备连接失败

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |

### onKitchenScaleReadyInteract

设备已准备完成，可以开始交互

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| code   | [int 详情见状态码列表](../Code.md#设备相关)       | 状态码     |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |

### onKitchenScaleDisconnected

设备已断开连接

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |