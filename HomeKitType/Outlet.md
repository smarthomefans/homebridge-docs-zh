# Outlet(插座)

[HAP-NodeJS 地址](https://github.com/KhaosT/HAP-NodeJS/blob/v0.4.50/lib/gen/HomeKitTypes.js#L3262)

必要
---
* `Characteristic.On` 开关状态,数据类型`bool`,对应值为`true` `false`
    * format 数据类型,bool
    * perms 权限 读,通知
* `Characteristic.OutletInUse ` 插座状态,是否使用中
    * format 数据类型,bool
    * perms 权限 读,通知


非必要 
---

* `Characteristic.Name` 名称