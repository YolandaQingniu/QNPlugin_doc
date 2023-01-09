# QNBPMachineData

血压计测量数据

#### 成员变量
| 名称        | 类型                       | 描述       |
|-----------|-----------------------------|-----------|
| timeStamp | String | 时间戳，单位s |
| userIndex | Int | 测量用户序号 |
| unit      | [QNBPMachineUnit](./QNBPMachineDeploy.md#qnbpmachineunit) | 当前单位 |
| systolicBP | String | 收缩压 |
| diastolicBP | String | 舒张压 |
| heartRate | String | 心率 |
| resultType | [QNBPMachineResultType](./QNBPMachineData.md#qnbpmachineresulttype) | 血压判断结果 |


#### QNBPMachineResultType
|名称  | 含义   |
| ------ |------|
|QNBPMachineResultTypeNormal_CHN | 正常血压（中国）   |
|QNBPMachineResultTypeNormalHighValue_CHN | 正常高值（中国） |
|QNBPMachineResultTypeFirstHighPressure_CHN | 1级高压（中国）   |
|QNBPMachineResultTypeSecondHighPressure_CHN | 2级高压（中国） |
|QNBPMachineResultTypeThirdHighPressure_CHN | 3级高压（中国）   |
|QNBPMachineResultTypeNormal_USA | 正常血压（美国）    |
|QNBPMachineResultTypeNormalHighValue_USA  | 血压高升（美国）  |
|QNBPMachineResultTypeFirstHighPressure_USA  | 1期高压（美国）    |
|QNBPMachineResultTypeSecondHighPressure_USA  | 2期高压（美国） |
|QNBPMachineResultTypeOptimalBloodPressure_EU  | 最佳血压（欧洲） |
|QNBPMachineResultTypeNormal_EU  | 正常血压（欧洲）   |
|QNBPMachineResultTypeNormalHighValue_EU  | 正常高值（欧洲） |
|QNBPMachineResultTypeFirstHighPressure_EU  | 1级高压（欧洲） |
|QNBPMachineResultTypeSecondHighPressure_EU  | 2级高压（欧洲） |
|QNBPMachineResultTypeThirdHighPressure_EU  | 3级高压（欧洲）|
|QNBPMachineResultTypeNormal_JPN  | 正常血压（日本）|
|QNBPMachineResultTypeNormalHighValue_JPN  | 正常高值（日本）|
|QNBPMachineResultTypeHighBloodPressure_JPN  | 血压高升（日本）|
|QNBPMachineResultTypeFirstHighPressure_JPN  | 1级高压（日本） |
|QNBPMachineResultTypeSecondHighPressure_JPN  | 2级高压（日本）|
|QNBPMachineResultTypeThirdHighPressure_JPN  | 3级高压（日本）|

