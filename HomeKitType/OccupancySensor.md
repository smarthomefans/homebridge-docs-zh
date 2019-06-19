# OccupancySensor (空间占用传感器)

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/master/lib/gen/HomeKitTypes.js#L3088)

>空间占用传感器是一款能针对不同类型用户应用检测空间或位置占用的应用。 例如根据占用情况控制照明和空调实现节能的应用。 室内占用传感器需要识别人，而不是其它移动的物体如纸张、植物、风扇。

必要
---
* `Characteristic.OccupancyDetected` 是否检测到空间有人占用
    * format 数据类型,UINT8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,通知


非必要 
---

* `Characteristic.StatusActive`  状态,数据(0,1)
* `Characteristic.StatusFault`
* `Characteristic.StatusTampered`
* `Characteristic.StatusLowBattery` 低电量警告,数据(0,1)
* `Characteristic.Name` 名称