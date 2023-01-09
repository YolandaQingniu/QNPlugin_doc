# QNHeightWeightScalePlugin
身高一体机设备管理

## API

### setScalePlugin

设置身高体重秤管理类
##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| plugin            | [QNPlugin](../QNPlugin/QNPlugin.md) | 基础管理类 |

##### 返回值
类型：[int 详情见状态码列表](../Code.md#初始化相关)

### setDeviceListener
设置设备监听器

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| deviceListener | [QNHeightWeightScaleDeviceListener](./QNHeightWeightScaleDeviceListener.md) | 设备设备监听器 |

### setDataListener
设置设备数据监听器

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| dataListener            | [QNHeightWeightScaleDataListener](./QNHeightWeightScaleDataListener)  | 设备监听器 |

### connectDevice
连接设备

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device  |  [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |
| operate  | [QNHeightWeightScaleOperate](./QNHeightWeightScaleOperate.md)  | 设置项 |

##### 返回值
类型：[int 详情见状态码列表](../Code.md#设备相关)

### cancelConnectDevice
断开设备连接

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| device  |  [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |

### setDeviceUnit
设置连接身高体重一体机重量单位与身高单位

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| weightUnit  | [QNWeightUnit](./QNHeightWeightScaleOperate.md)  | 重量单位 |
| heightUnit  | [QNHeightUnit](./QNHeightWeightScaleOperate.md)  | 身高单位 |
| device  |  [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |


##### 返回值
类型：[int 详情见状态码列表](../Code.md#设备相关)


### setMeasureUser
设置测量用户相关信息

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| user  | [QNHeightWeightUser](./QNHeightWeightUser.md)  | 用户信息 |
| device  |  [QNHeightWeightScaleDevice](./QNHeightWeightScaleDevice.md)   | 身高一体机设备 |

##### 返回值
类型：[int 详情见状态码列表](../Code.md)


### getWeightLb
单位转换:  kg转lb

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| weight  | String                   | 测量数据返回的[weight](./QNHeightWeightScaleData.md)字符串 |

##### 返回值
| 类型                 | 说明                |
| :---------------------- | :------------------------- |
| String                   | 对应lb单位数值的字符串,一位有效数字 |


### getWeightJin:
单位转换:  kg转斤

##### 参数
| 名称       | 类型                 | 说明                |
| :----------| :--------------- | :------------------------- |
| weight            | String                   | 测量数据返回的[weight](./QNHeightWeightScaleData.md)字符串 |

##### 返回值
| 类型                 | 说明                |
| :---------- | :------------------------- |
| String      | 对应斤单位数值的字符串,一位有效数字 |

### getWeightStLb:
单位转换:  kg转StLb

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| weight             | String                   | 测量数据返回的[weight](./QNHeightWeightScaleData.md)字符串 |

##### 返回值
| 类型                 | 说明                |
| :---------------------- | :------------------------- |
| String [ ]     | \[0] 对应St单位数值的字符串 ，整形 ； \[1] 对应Lb单位数值的字符串， 一位有效数字|

### getWeightSt:
单位转换:  kg转st

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| weight          | String                   | 测量数据返回的[weight](./QNHeightWeightScaleData.md)字符串 |

##### 返回值
| 类型                 | 说明                |
| :------------------ | :------------------------- |
| String              | 对应st单位数值的字符串,两位有效数字 |

### getHeightFtIn:
单位转换:  cm转FtIn

##### 参数
| 名称          | 类型                 | 说明                |
| :------------ | :---------------------- | :------------------------- |
| height          | String                   | 测量数据返回的[height](./QNHeightWeightScaleData.md)字符串 |

##### 返回值
| 类型                 | 说明                |
| :---------------------- | :------------------------- |
| String [ ]                  | \[0]  对应Ft单位数值的字符串 ，整形 ； \[1] 对应In单位数值的字符串， 一位有效数字|