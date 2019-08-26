# Fanv2 (风扇)

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/v0.4.50/lib/gen/HomeKitTypes.js#L2905)

必要
---
* `Characteristic.Active` 开关状态, 1打开,0关闭
    * format 数据类型,uint8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,写,通知


非必要 
---

* `Characteristic.Name` 名称
* `Characteristic.SwingMode  ` 是否摆动
    * format 数据类型,UINT8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,写,通知
* `Characteristic.LockPhysicalControls   `  童锁
    * format 数据类型,UINT8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,写,通知
      
* `Characteristic.TargetFanState   `  风扇模式,自动还收手动
    * format 数据类型,UINT8
    * maxValue 最大值 1
    * minValue 最小值 0
    * perms 权限 读,写,通知
* `Characteristic.CurrentFanState    ` 风扇状态,`不活跃` `空闲` `吹风中`
    * format 数据类型,浮点数
    * unit 单位: UINT8
    * maxValue 最大值 2
    * minValue 最小值 0
    * minStep 最小进位 1
    * perms 权限 读,写,通知

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