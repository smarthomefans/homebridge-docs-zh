# Thermostat(恒温器) 

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/master/lib/gen/HomeKitTypes.js#L3443)

必要
---
* `Characteristic.CurrentTemperature` 当前温度
    * format 数据类型,浮点数
    * unit 单位: celsius(摄氏度)
    * maxValue 最大值 100
    * minValue 最小值 0
    * minStep 最小进位 0.1
    * perms 权限 读,通知


* `Characteristic.CurrentHeatingCoolingState ` 当前的状态状态, `关闭` `制热` `制冷`
    * format 数据类型,UINT8
    * maxValue 最大值 2
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知

```js
// The value property of CurrentHeatingCoolingState must be one of the following:
Characteristic.CurrentHeatingCoolingState.OFF = 0;
Characteristic.CurrentHeatingCoolingState.HEAT = 1;
Characteristic.CurrentHeatingCoolingState.COOL = 2;
```

* `Characteristic.TargetHeatingCoolingState ` 设置状态, `关闭` `制热` `制冷`  `自动`
    * format 数据类型,UINT8
    * maxValue 最大值 3
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知

```js
// The value property of TargetHeatingCoolingState must be one of the following:
Characteristic.TargetHeatingCoolingState.OFF = 0;
Characteristic.TargetHeatingCoolingState.HEAT = 1;
Characteristic.TargetHeatingCoolingState.COOL = 2;
Characteristic.TargetHeatingCoolingState.AUTO = 3;
```

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

非必要 
---
* `Characteristic.Name` 名称

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

* `Characteristic.CurrentRelativeHumidity` 当前湿度
    * format 数据类型,浮点数
    * unit 单位: %
    * maxValue 最大值 100
    * minValue 最小值
    * minStep 最小进位 1
    * perms 权限 读,通知

    
* `Characteristic.TargetRelativeHumidity` 设置的湿度
    * format 数据类型,浮点数
    * unit 单位: %
    * maxValue 最大值 100
    * minValue 最小值
    * minStep 最小进位 1
    * perms 权限 读,通知