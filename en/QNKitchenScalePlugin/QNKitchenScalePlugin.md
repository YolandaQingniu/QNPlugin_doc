# QNKitchenPlugin

厨房秤设备管理

## API

### setKitchenPlugin

设置厨房秤管理类

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
| deviceListener | [QNKitchenScaleDeviceListener](./QNKitchenScaleDeviceListener.md) | 设置设备监听器 |

### setDataListener

设置设备数据监听器

##### 参数

| 名称         | 类型                                                         | 说明           |
| :----------- | :----------------------------------------------------------- | :------------- |
| dataListener | [QNKitchenScaleDataListener](./QNKitchenScaleDataListener.md) | 设置数据监听器 |

### connectDevice

连接设备

##### 参数

| 名称    | 类型                                                | 说明       |
| :------ | :-------------------------------------------------- | :--------- |
| operate | [QNKitchenScaleOperate](./QNKitchenScaleOperate.md) | 设置项     |
| device  | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md)   | 厨房秤设备 |

##### 返回值

类型：[int 详情见状态码列表](../Code.md#设备相关)

### cancelConnectDevice

断开设备连接

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |

### setDeviceUnit

设置设备单位

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |
| unit   | [QNUnit](./QNKitchenScaleData.md#QNUnit)          | 单位       |

##### 返回值

类型：[int 详情见状态码列表](../Code.md#初始化相关)

### setDeviceShelling

设置设备秤端去皮

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |

##### 返回值

类型：[int 详情见状态码列表](../Code.md#初始化相关)

### setDeviceShutDown

设置设备称端关机

##### 参数

| 名称   | 类型                                              | 说明       |
| :----- | :------------------------------------------------ | :--------- |
| device | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md) | 厨房秤设备 |

##### 返回值

类型：[int 详情见状态码列表](../Code.md#初始化相关)

### setDeviceStandbyTime

设置设备亮屏时长

##### 参数

| 名称        | 类型                                                         | 说明       |
| :---------- | :----------------------------------------------------------- | :--------- |
| standbyTime | [QNKitchenScaleStandbyTimeType](./QNKitchenScaleDevice.md#QNKitchenScaleStandbyTimeType) | 亮屏时长   |
| device      | [QNKitchenScaleDevice](./QNKitchenScaleDevice.md)            | 厨房秤设备 |

##### 返回值

类型：[int 详情见状态码列表](../Code.md#初始化相关)



### getWeightWithUnit:weight:numberType

单位转换

##### 参数

| 名称       | 类型                                                         | 说明                                                       |
| :--------- | :----------------------------------------------------------- | :--------------------------------------------------------- |
| unit       | [QNUnit](./QNKitchenScaleData.md#QNUnit)                     | 传入目标单位                                               |
| weight     | String                                                       | 测量数据返回的[weight](./QNHeightWeightScaleData.md)字符串 |
| numberType | [QNKitchenScaleNumberType](./QNKitchenScaleDevice.md#QNKitchenScaleNumberType) | 数据的精度类型                                             |

##### 返回值

| 类型   | 说明                                                     |
| :----- | :------------------------------------------------------- |
| String | 对应单位数值的字符串，根据数据精度类型来决定保留几位小数 |

### 