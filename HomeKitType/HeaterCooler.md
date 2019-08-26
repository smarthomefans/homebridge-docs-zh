# HeaterCooler(空调) 

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/v0.4.50/lib/gen/HomeKitTypes.js#L2990)


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

* `Characteristic.CurrentHeaterCoolerState` 空调状态,`不活跃` `空闲` `制热` `制冷`
    * format 数据类型,UINT8
    * maxValue 最大值 3
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知

```js
// The value property of CurrentHeaterCoolerState must be one of the following:
Characteristic.CurrentHeaterCoolerState.INACTIVE = 0;
Characteristic.CurrentHeaterCoolerState.IDLE = 1;
Characteristic.CurrentHeaterCoolerState.HEATING = 2;
Characteristic.CurrentHeaterCoolerState.COOLING = 3;
```

* `Characteristic.TargetHeaterCoolerState ` 空调状态, `自动` `制热` `制冷`
    * format 数据类型,UINT8
    * maxValue 最大值 2
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知

```js
// The value property of TargetHeaterCoolerState must be one of the following:
Characteristic.TargetHeaterCoolerState.AUTO = 0;
Characteristic.TargetHeaterCoolerState.HEAT = 1;
Characteristic.TargetHeaterCoolerState.COOL = 2;
```

* `Characteristic.CurrentTemperature` 当前温度
    * format 数据类型,浮点数
    * unit 单位: celsius(摄氏度)
    * maxValue 最大值 100
    * minValue 最小值 0
    * minStep 最小进位 0.1
    * perms 权限 读,通知

非必要 
---
* `Characteristic.Name` 名称
* `Characteristic.SwingMode  ` 是否扫风
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

* `Characteristic.CoolingThresholdTemperature`  制冷的温度和自动时候的最低温度
    * format 数据类型,浮点数
    * unit 单位: celsius(摄氏度)
    * maxValue 最大值 35
    * minValue 最小值 10
    * minStep 最小进位 0.1
    * perms 权限 读,通知

* `Characteristic.HeatingThresholdTemperature`  制热的温度和自动时候的最高温度
    * format 数据类型,浮点数
    * unit 单位: celsius(摄氏度)
    * maxValue 最大值 25
    * minValue 最小值 0
    * minStep 最小进位 0.1
    * perms 权限 读,通知

* `Characteristic.TemperatureDisplayUnits   `  单位，摄氏度或华氏温度
    * format 数据类型,UINT8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,写,通知
```js
// The value property of TemperatureDisplayUnits must be one of the following:
Characteristic.TemperatureDisplayUnits.CELSIUS = 0;
Characteristic.TemperatureDisplayUnits.FAHRENHEIT = 1;
```

* `Characteristic.RotationSpeed  ` 转速, 速度为0时关闭
    * format 数据类型,浮点数
    * unit 单位: %
    * maxValue 最大值 100
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知