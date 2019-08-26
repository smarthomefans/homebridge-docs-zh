# Lightbulb  (灯)

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/v0.4.50/lib/gen/HomeKitTypes.js#3132)

必要
---
* `Characteristic.On` 开关状态,数据类型`bool`,对应值为`true` `false`
    * format 数据类型,bool
    * perms 权限 读,写,通知


非必要 
---
* `Characteristic.Name` 名称
* `Characteristic.Brightness` 亮度
    * format 数据类型,int
    * unit 单位  %
    * maxValue 最大值 100
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,通知

* `Characteristic.Hue` 颜色
    * format 数据类型,FLOAT
    * unit 单位  ARC_DEGREE
    * maxValue 最大值 360
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,通知

* `Characteristic.Saturation` 饱和度
    * format 数据类型,int
    * unit 单位  %
    * maxValue 最大值 100
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,通知

* `Characteristic.ColorTemperature` 色温
    * format 数据类型,UINT32
    * maxValue 最大值 500
    * minValue 最小值 140
    * minStep 最小进位 1
    * perms 权限 读,通知



