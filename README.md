### 停止更新
由于这个方法属于破坏了ss的sip003的接口规则来实现集成kcptun，不符合ss的接口规则。

并且这个方法对ss-win的改动比较多，不方便后续维护，也可能是因为我比较懒:)

当然目前（截止2018-4-26）这个版本还是可以继续使用的

我将在一个项目中实现ss建议的接口规则，来使ss支持kcptun插件（即实现一个ss与kcptun之间的接口适配器）。



Shadowsocks for Windows With kcptun
=======================
### 简介
从[shadowsocks-windows]`版本46d40fe`克隆过来，简单修改了插件功能，使其支持kcptun。

通过[shadowsocks-plugin]了解到原本的shadowsocks插件功能目的是支持[simple-obfs]，该插件本身功能是将ss通讯数据进行混淆。

原本[shadowsocks-plugin]使用SIP003`对其还不是很了解:(`接口，但是经过测试无法正常使用kcptun，所以将原本代码进行简单修改。



### 其他
* shadowsocks-windows:https://github.com/shadowsocks/shadowsocks-windows
* shadowsocks-plugin:https://github.com/shadowsocks/shadowsocks-org/wiki/Plugin
* kcptun:https://github.com/xtaci/kcptun

[shadowsocks-windows]: https://github.com/shadowsocks/shadowsocks-windows
[shadowsocks-plugin]:https://github.com/shadowsocks/shadowsocks-org/wiki/Plugin
[simple-obfs]:https://github.com/shadowsocks/simple-obfs
