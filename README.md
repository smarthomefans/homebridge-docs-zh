# HomeBridge Docs(HomeBridge中文文档)

起因  
---
在我学习使用`hb`的过程中,发现不明白`hb`的地方发现只能通过查看代码解决.我发现这很不方便也不利于国内小伙伴学习使用.所以这里做了一些相关的我学习的记录,用来说明`hb`设备的属性,希望对大家有用.

HomeBridge 是什么?  
---
Homebridge is a lightweight NodeJS server that emulates the iOS HomeKit API；  
简单来说就是一个`nodejs`的服务可以模拟出`homekit api`,让我们接入任意自己想接入的设备.

HomeBridge 插件会发布 Accessories 和 Platforms，Accessories是一个独立的设备，而Platforms是这些设备所连接的同一个平台/同一组设备.



设备基本属性  
---
一个设备在`homekit`里面必须含有一下属性
* `Identify` 唯一标识
* `Manufacturer` 制造商,也就是厂家
* `Model`  设备型号
* `Name`  设备名称
* `SerialNumber` 串号
* `FirmwareRevision` 固件版本

还有另外两个比较重要的属性`username`和`pin码`,前者是我们常规理解的mac地址一样,后者是我们连接设备需要使用的一串数字

