# QNScaleStoredData
Home scales store data

##### Member variable
| name          | type                 | description                |
| ------ | ------ | ------ |
| isDataComplete | Bool | Data integrity |
| timeStamp | String | Time stamp, unit s |
| hmac | String |Data encryption string  |
| weight | String |Weight, a two-digit significant value in kg |

### getScaleData

Obtain measurement data details

##### parameter
nil

##### Return value
| name          | type                 | description                |
| ------ | ------ | ------ |
| scaleData | [QNScaleData](../Model/QNScaleData.md)  | Measurement data |