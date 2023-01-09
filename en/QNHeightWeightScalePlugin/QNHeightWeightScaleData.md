# QNHeightWeightScaleData
身高一体机测量数据

#### 成员变量
| 名称 | 类型 | 描述 | 
| ------ | ------ | ------ |
| isDataComplete | Bool | 数据是否完整 |
| deviceMode | [QNHeightWeightMode](./QNHeightWeightScaleData.md#qnheightweightmode) | 身高一体机测量模式 |
| timeStamp | String | 时间戳，单位s |
| hmac | String |数据加密字符串  |
| user | [QNHeightWeightUser](./QNHeightWeightUser.md)  | 用户信息  |
| weight | String |体重，单位kg 两位有效数值 |
| height | String | 身高，单位cm  两位有效数值  |
| bmi | String |BMI  一位有效数值 |
| bodyFatRate | String |体脂肪率 一位有效数值 |
| subcutaneousFatRate | String |皮下脂肪率 一位有效数值 |
| visceralFatLevel | String |内脏脂肪等级 一位有效数值 |
| bodyWaterRate | String |身体水分率 一位有效数值 |
| skeletalMuscleRate | String |骨骼肌率 一位有效数值 |
| boneMass | String |骨量 两位有效数值 |
| BMR | String |基础代谢量  |
| bodyType | String |体型  |
| proteinRate | String |蛋白质率 一位有效数值 |
| leanBodyMass | String |去脂体重  两位有效数值|
| muscleMass | String |肌肉量 两位有效数值 |
| bodyAge | String |体年龄  |
| healthScore | String |健康分数  |
| fattyLiverRiskLevel | String |脂肪肝风险等级  |
| bodyFatMass | String |脂肪量 两位有效数值 |
| obesity | String |肥胖度  |
| bodyWaterMass | String |含水量 两位有效数值 |
| proteinMass | String |蛋白质量 两位有效数值 |
| mineralLevel | String |无机盐状况（low; stand; enough）|
| dreamWeight | String |理想视觉体重 两位有效数值 |
| standWeight | String |标准体重  两位有效数值|
| weightControl | String |体重控制量 两位有效数值 |
| bodyFatControl | String |脂肪控制量 两位有效数值 |
| muscleMassControl | String |肌肉控制量 两位有效数值 |
| muscleRate | String |肌肉率  一位有效数值 |


#### makeDataComplete:
完善测量数据
##### 参数
| 名称 | 类型 | 描述 |
| ------ | ------ | ------ |
| user | [QNHeightWeightUser](./QNHeightWeightUser.md)  | 用户信息 |

##### 返回值
| 名称 | 类型 | 描述 |
| ------ | ------ | ------ |
| scaleData | QNHeightWeightScaleData | 测量数据 |


#### QNHeightWeightMode
|名称  |含义|
| ------ | ------ |
|HeightWeight  | 身高体重模式 |
|HeightBodyFat  | 身高体脂模式 |
