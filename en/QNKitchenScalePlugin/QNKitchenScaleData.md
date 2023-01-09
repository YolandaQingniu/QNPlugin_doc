# QNKitchenScaleData

厨房秤测量数据

#### 成员变量

| 名称                | 类型                                     | 描述                      |
| ------------------- | :--------------------------------------- | ------------------------- |
| weight              | String                                   | 重量，单位kg 两位有效数值 |
| unit                | [QNUnit](./QNKitchenScaleData.md#QNUnit) | 单位                      |
| timeStamp           | String                                   | 时间戳，单位秒            |
| isShellingFlag      | Bool                                     | 是否去皮                  |
| isOverWeightFlag    | Bool                                     | 是否超载                  |
| isReverseWeightFlag | Bool                                     | 是否是负体重              |
| isStableFlag        | Bool                                     | 是否稳定                  |

#### QNUnit

| 名称         | 含义     |
| :----------- | :------- |
| QNUnitG      | 克       |
| QNUnitML     | 毫升     |
| QNUnitOZ     | 盎司     |
| QNUnitLBOZ   | 磅       |
| QNUnitMilkML | 牛奶称量 |

#### 
