# Fan(风扇)

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/v0.4.50/lib/gen/HomeKitTypes.js#L2885)

必要
---
* `Characteristic.On` 开关状态,数据类型`bool`,对应值为`true` `false`
    * format 数据类型,bool
    * perms 权限 读,通知


非必要 
---

* `Characteristic.Name` 名称
* `Characteristic.RotationDirection  ` 风扇旋转方向,顺时针和逆时针
    * format 数据类型,int
    * maxValue 最大值 1
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知
* `Characteristic.RotationSpeed  ` 转速, 速度为0时关闭
    * format 数据类型,浮点数
    * unit 单位: %
    * maxValue 最大值 100
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知