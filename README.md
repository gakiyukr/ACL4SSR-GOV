# ACL4SSR-GOV 规则

* 项目基于CC-BY-SA-4.0协议发布  [![CC-BY-SA-4.0](https://licensebuttons.net/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/deed.zh)
* 本规则基于 ACL4SSR 完善
* 添加了 Google One VPN 相关规则

## 如何使用

直接在配置转换网站中，将 [本规则 ](https://raw.githubusercontent.com/gakiyukr/ACL4SSR-GOV/master/ACL4SSR-GOV.ini)作为远程配置使用。


## Clash规则

主要文件在 Clash 文件夹下，只是一些规则碎片，可以配合一些订阅转换进行使用。

具体怎么使用需要看对应 Proxy 软件配置是怎么写的，还要请大家阅读你所使用的 Proxy 软件文档，看看否能使用。

示例：项目里 `/Clash/config/` 目录下存放的是 [subconverter ](https://github.com/tindy2013/subconverter/blob/master/README-cn.md#外部配置)的 配置示例

| 文件                   | 类型                 | 解释                                                         |
| ---------------------- | -------------------- | :----------------------------------------------------------- |
| BanAD.list             | 规则碎片-去广告      | 只包含常见广告关键字、广告联盟。无副作用，放心使用           |
| BanProgramAD.list      | 规则碎片-去广告      | 包含常用应用的各种去广告规则。可能有轻微副作用，可放心使用。（如果网站功能和广告冲突，会删掉去广告规则） |
| BanEasyListChina.list  | 规则碎片-去广告      | AdblockPlus 中的中国所有的屏蔽域名                           |
| LocalAreaNetwork.list  | 规则碎片-直连        | 本地地址和路由器直连域名啥的                                 |
| ChinaDomain.list       | 规则碎片-直连        | 国内常见域名、直连 CDN 等。（很全，常用网址都有）            |
| ChinaCompanyIp.list    | 规则碎片-直连        | 国内 BAT 公司及云服务厂商的 IP 段。所有在该云服务上的网站都可以直连。比如你网站在阿里云香港都可以直连。 |
| ChinaIp.list           | 规则碎片-直连        | IPIP 的国内地址段。比 GeoIp 更好。电脑性能好，可以引入       |
| Download.list          | 规则碎片-直连        | 一些下载用的域名                                             |
| Apple.list             | 规则碎片             | Apple 的所有域名                                             |
| Microsoft.list         | 规则碎片             | Microsoft 的所有域名                                         |
| OneDrive.list          | 规则碎片             | OneDrive                                                     |
| GoogleCN.list          | 规则碎片-直连        | Google 在中国能直连的网址列表                                |
| Telegram.list          | 规则碎片-代理        | Telegram 的所有域名                                          |
| Netflix.list           | 规则碎片-代理        | Netflix 的所有域名                                           |
| ProxyGFWlist.list      | 规则碎片-代理        | GFW 的全量列表                                               |
| ProxyLite.list         | 规则碎片-代理        | 比较精简的代理列表，包含常用的，以及被污染的域名             |
| GeneralClashConfig.yml | clash配置文件        | 放行一堆国内的常用域名，配合系统代理更牛逼。 配置很全，自带中文注释。可以自行使用 |
| pref.ini               | subconverter配置文件 | 更改了一些基础配置，将规则变成ACL4SSR                        |
| GOV.list               | 规则碎片-代理        | Google One VPN 的相关域名                                    |
| GOV-IP.list            | 规则碎片-代理        | Google One VPN 的相关 IP                                     |



# License		
[![](https://licensebuttons.net/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/deed.zh)
* CC-BY-SA-4.0
