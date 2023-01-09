# QNHeightWeightScaleOperate
身高一体机设置

#### 成员变量
| 名称 | 类型 | 描述 | 
| ------ | ------ | ------ |
| weightUnit | QNWeightUnit | 体重单位 |
| heightUnit | QNHeightUnit | 身高单位  | 

#### QNWeightUnit
|名称  |含义|
|:--|:--|
|QNWeightUnitKg  | kg |
|QNWeightUnitLb  | lb |
|QNWeightUnitJin  | 斤，如果秤不支持斤，则自动设置为kg |
|QNWeightUnitSt  | st，如果秤不支持st，则自动设置为就显示lb |
|QNWeightUnitStLb  | st:lb，如果秤不支持st:lb，则自动设置为就显示lb |

#### QNHeightUnit
|名称  |含义|
|:--|:--|
|QNHeightUnitCm  | 厘米 |
|QNHeightUnitFt  | 英寸 |
