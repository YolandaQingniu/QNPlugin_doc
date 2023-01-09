# QNKitchenScaleDevice

厨房秤设备

#### 成员变量

| 名称     | 类型   | 描述         |
| -------- | ------ | ------------ |
| mac      | String | mac地址      |
| rssi     | int    | 信号强度     |
| bleName  | String | 蓝牙名       |
| modelId  | String | 设备类型标识 |
| scaleVer | String | 硬件版本     |
| bleVer   | String | 软件版本     |



#### QNKitchenScaleStandbyTimeType

| 名称                              | 含义                          |
| --------------------------------- | ----------------------------- |
| QNKitchenScaleStandbyTimeType120S | 待机时间2分钟（ 默认 ）=120秒 |
| QNKitchenScaleStandbyTimeType210S | 待机时间3.5分钟 = 210秒       |
| QNKitchenScaleStandbyTimeType300S | 待机时间5分钟 = 300秒         |



#### QNKitchenScaleNumberType

| 名称                               | 含义     |
| ---------------------------------- | -------- |
| QNKitchenScaleNumberTypeInteger    | 整型     |
| QNKitchenScaleNumberTypeOneDecimal | 一位小数 |
| QNKitchenScaleNumberTypeTwoDecimal | 二位小数 |



#### QNKitchenScaleRangeType

| 名称                       | 含义  |
| -------------------------- | ----- |
| QNKitchenScaleRangeType3KG | 0~3kg |
| QNKitchenScaleRangeType5KG | 0~5kg |



### getDeviceSupportShelling

获取设备是否支持去皮

##### 参数

   无

##### 返回值

| 类型 | 描述         |
| ---- | ------------ |
| Bool | 是否支持去皮 |

### getDeviceSupportShutDown

获取设备是否支持关机

##### 参数

   无

##### 返回值

| 类型 | 描述         |
| ---- | ------------ |
| Bool | 是否支持关机 |

### getDeviceSupportStandbyTime

获取设备是否支持设置亮屏时长

##### 参数

   无

##### 返回值

| 类型 | 描述                 |
| ---- | -------------------- |
| Bool | 是否支持设置亮屏时长 |

### getDeviceStandbyTime

获取设备亮屏时长

##### 参数

   无

##### 返回值

| 类型                          | 描述     |
| ----------------------------- | -------- |
| QNKitchenScaleStandbyTimeType | 亮屏时长 |

### getDeviceNumberType

获取设备数据精度类型

##### 参数

   无

##### 返回值

| 类型                     | 描述             |
| ------------------------ | ---------------- |
| QNKitchenScaleNumberType | 测量数据精度类型 |

### getDeviceRangeType

获取设备量程

##### 参数

   无

##### 返回值

| 类型                    | 描述     |
| ----------------------- | -------- |
| QNKitchenScaleRangeType | 设备量程 |

### getDeviceUnitSupportedList

获取设备前支持单位列表

##### 参数

   无

##### 返回值

| 类型  | 描述                                                         |
| ----- | ------------------------------------------------------------ |
| Array | 当前支持单位列表 数组长度为零时，代表当前设备无法读取支持单位列表 |
