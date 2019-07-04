# ContactSensor (门窗传感器)

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/master/lib/gen/HomeKitTypes.js#L2821)

必要
---
* `Characteristic.ContactSensorState` 状态, 对应值为`关闭: 0` `打开: 1`
    * format 数据类型,UINT8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,通知
```js
// The value property of ContactSensorState must be one of the following:
Characteristic.ContactSensorState.CONTACT_DETECTED = 0;
Characteristic.ContactSensorState.CONTACT_NOT_DETECTED = 1;
```

非必要 
---

* `Characteristic.StatusActive`  状态,数据(0,1)
* `Characteristic.StatusFault`
* `Characteristic.StatusTampered`
* `Characteristic.StatusLowBattery` 低电量警告,数据(0,1)
* `Characteristic.Name` 名称