# QNUser

Yolanda user object

### attribute

| name          | type  |  Whether it is necessary  | description                                                                                               |
| :------------ | :----- | :-----| :--------------------------------------------------------------------------------------------------------------------------- |
| height        | int    | Y | Height, unit is cm, minimum 40, maximum 240                                                                                                 |
| gender        | String | Y | Gender, male: male, female: female                                                                                                     |
| birthday      | Date   | Y | Birthday, used to calculate age, date precision accurate to days, calculate the age range is 3~80, more than this range, equal to the upper or lower limit.                                  |
| athleteType   | int    | Y | 是否为运动员模式（0 为普通算法,1 为运动员算法)，该字段只在年龄大于或等于 18 岁时才生效                                           |
| clothesWeight | double | Y | 单位: KG <br>衣物重量，设置该值时，测量体重值返回的将是减去衣物重量的值。<br>衣物重量不可超过体重的一半,否则将会忽略超过的值     |
| index         | int    | N | 用户秤设备专用，秤端该用户索引。该值不赋值时, 秤链接成功后会进行注册称端用户 ,该值由向秤注册用户成功时，秤端返回。需要保存到服务器 访问用户时需要传递  |