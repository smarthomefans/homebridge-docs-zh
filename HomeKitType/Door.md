# Door (门)

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/v0.4.50/lib/gen/HomeKitTypes.js#L2843)


必要
---
* `Characteristic.CurrentPosition    `  当前门的位置
    * format 数据类型,UINT8
    * unit 单位: PERCENTAGE
    * maxValue 最大值 100
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知

* `Characteristic.PositionState    `  门的状态， `关闭中` `打开中` `停止`
    * format 数据类型,浮点数
    * unit 单位: UINT8
    * maxValue 最大值 2
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,通知

```js
// The value property of PositionState must be one of the following:
Characteristic.PositionState.DECREASING = 0;
Characteristic.PositionState.INCREASING = 1;
Characteristic.PositionState.STOPPED = 2;
```

* `Characteristic.TargetPosition    `  设定门的位置
    * format 数据类型,UINT8
    * unit 单位: PERCENTAGE
    * maxValue 最大值 100
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知


非必要 
---

* `Characteristic.Name` 名称
* `Characteristic.HoldPosition` 不晓得这么描述
* `Characteristic.ObstructionDetected` 不晓得这么描述
