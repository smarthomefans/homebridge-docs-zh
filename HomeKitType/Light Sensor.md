# Light Sensor (光照传感器)

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/master/lib/gen/HomeKitTypes.js#L3100)

必要
---
* `Characteristic.CurrentAmbientLightLevel` 光照强度
    * format 数据类型,FLOAT
    * unit 单位  lux
    * maxValue 最大值 100000
    * minValue 最小值 0.0001
    * perms 权限 读,通知


非必要 
---

* `Characteristic.StatusActive`  状态,数据(0,1)
* `Characteristic.StatusFault`
* `Characteristic.StatusTampered`
* `Characteristic.StatusLowBattery` 低电量警告,数据(0,1)
* `Characteristic.Name` 名称