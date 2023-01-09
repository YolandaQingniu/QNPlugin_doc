# QNRulerDeviceListener
设备相关事件监听器

## API

### onDiscoverRulerDevice
搜索到设备的事件回调

##### 参数
| 名称          | 类型                                             | 说明    |
| :------------ |:-----------------------------------------------|:------|
| device  | [QNRulerDevice](./QNRulerDevice.md) | 围度尺设备 |

### onRulerConnectedSuccess
设备连接成功回调
##### 参数
| 名称          | 类型                 | 说明                |
| :------------ |:-----------------------------------------------|:------|
| device  | [QNRulerDevice](./QNRulerDevice.md) | 围度尺设备 |

### onRulerConnectFail
设备连接失败

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device  | [QNRulerDevice](./QNRulerDevice.md) | 围度尺设备 |

### onRulerReadyInteract
设备已准备完成，可以开始交互

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| code       | [int 详情见状态码列表](../Code.md#设备相关)                  | 状态码 |
| device  | [QNRulerDevice](./QNRulerDevice.md) | 围度尺设备 |

### onRulerDisconnected
设备已断开连接
##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device  | [QNRulerDevice](./QNRulerDevice.md) | 围度尺设备 |