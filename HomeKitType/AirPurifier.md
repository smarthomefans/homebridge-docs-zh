# Air Purifier (空气净化器)

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/master/lib/gen/HomeKitTypes.js#L2677)


必要
---
* `Characteristic.Active` 开关状态, 1打开,0关闭
    * format 数据类型,uint8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,写,通知
``` js
// The value property of Active must be one of the following:
Characteristic.Active.INACTIVE = 0;
Characteristic.Active.ACTIVE = 1;
```

* `Characteristic.CurrentAirPurifierState    ` 风扇状态,`不活跃` `空闲` `开启状态`
    * format 数据类型,UINT8
    * maxValue 最大值 2
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知
```js
// The value property of CurrentAirPurifierState must be one of the following:
Characteristic.CurrentAirPurifierState.INACTIVE = 0;
Characteristic.CurrentAirPurifierState.IDLE = 1;
Characteristic.CurrentAirPurifierState.PURIFYING_AIR = 2;
```

* `Characteristic.TargetAirPurifierState  `  模式,自动还收手动
    * format 数据类型,UINT8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,写,通知
```js
// The value property of TargetAirPurifierState must be one of the following:
Characteristic.TargetAirPurifierState.MANUAL = 0;
Characteristic.TargetAirPurifierState.AUTO = 1;
```



非必要 
---
* `Characteristic.Name` 名称
* `Characteristic.SwingMode  ` 是否摆动
    * format 数据类型,UINT8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,写,通知
```js
// The value property of SwingMode must be one of the following:
Characteristic.SwingMode.SWING_DISABLED = 0;
Characteristic.SwingMode.SWING_ENABLED = 1;
```
* `Characteristic.LockPhysicalControls   `  童锁
    * format 数据类型,UINT8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,写,通知
```js
// The value property of LockPhysicalControls must be one of the following:
Characteristic.LockPhysicalControls.CONTROL_LOCK_DISABLED = 0;
Characteristic.LockPhysicalControls.CONTROL_LOCK_ENABLED = 1;
```
* `Characteristic.RotationSpeed  ` 转速, 速度为0时关闭
    * format 数据类型,浮点数
    * unit 单位: %
    * maxValue 最大值 100
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知