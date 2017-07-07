# lhie1/Surge 用户手册

### lhie1/Surge 简介

`lhie1/Surge` 最早是基于 `[scomper/surge.conf](https://gist.github.com/scomper/915b04a974f9e11952babfd0bbb241a8)` 定制修改而来，鄙人已维护两年有余。

---
* 支持应用
    * Surge
    * Shadowrocket
* 导入方式
    * ~~URL~~
    * Workflow(#workflow)
    * [~~在线更新（暂弃）~~](https://github.com/lhie1/RuleList)
* [功能](#功能)

---

### 功能
* 自动代理 / 全局代理
* 解决本地 DNS 可能带来的干扰
* 可突破部分内网限制（公司、学校）
* 拦截常用应用程序的行为分析
* 拦截常用应用程序的数据统计
* 拦截常用应用程序的隐私跟踪
* 拦截各大购物网站的运营商劫持
* 屏蔽部分应用程序的启动广告
* 屏蔽部分运营商劫持网页弹出的流量统计
* 屏蔽部分运营商劫持网页弹出的漂浮球广告
* 屏蔽常用视频广告
* 屏蔽常用网站广告、其他流媒体网站广告
* 所有国内网站直线连接
* Apple 服务加速（App Store、Apple Music、Apple流媒体、iCloud备份、iCloud Drive、iTunes 等）
* 国外常用网站加速（Google/Youtube/Twitter/Facebook/instagram/wikipedia/Github 等）

### Workflow

* User Data
    * 自定义[Proxy]节点
    * 自动根据[Proxy]内容生成[Proxy Group]
    * 自定义添加[Rule]规则
    * 自定义添加[Host]规则
    * 自定义添加[URL Rewrite]规则
    * 自定义添加[SSID Setting]规则
    * 自定义删除规则（All）
* Rule OTA
    * Special_Proxy
        * AuthKey
        * Google
        * Netflix
        * MytvSUPER
    * Features_Module
        * Adblocker
        * TestFlight
        * Emoji
    * 自动更新
    * 自动修复 module 模块
    * 生成规则

#### User Data

Download：https://workflow.is/workflows/7100cebf06ad4adead9aac76e45e50b2

#### Rule OTA

Download：https://workflow.is/workflows/1178156c473b45cb9b10205b39e46faa




    Surge 视频教程：https://youtu.be/IRJOAnPZWJM

    Shadowrocket 视频教程：https://youtu.be/nPFHi99PYww

    PS：基于 爱兔联盟.com 提供的节点快速获取并使用



    Hosts：https://async.be/Rule/Basic/Hosts
    （免服务器 / 自动更新 ／ 支持 google、instagram、twitter 等主流外网）

    Telegram：http://t.me/RuleNews
    （更新日志 / 新内容发布 ／ 更方便快捷获取更新内容 ／ 进阶功能教程）

🤖️ Android SSR ACL

    ACL4SSR：https://github.com/ACL4SSR/ACL4SSR

🈲️ 浏览器广告

    全平台：Adguard - https://adguard.com/en/welcome.html



# line

About | Link |
---------|:---------:
新浪微博 | [@lhie1](http://www.weibo.com/1748625493)
Telegram 讨论组| https://telegram.me/lhie1x
Telegram 通知频道| http://t.me/RuleNews
购买翻墙服务| [爱兔联盟（通往新宇宙的船票）](https://爱兔联盟.com)

Tutor | Raw |
---------|:---------:
@Eval | https://twitter.com/OAuth4
@Scomper| https://medium.com/@scomper
@Neurogram| http://www.taguage.com/user?id=181456
@suisr9255| -
@Hackl0us| https://github.com/Hackl0us


# Q&A

### ☁️ Proxy & 🔰 Proxy & 🍎 Proxy

    ☁️ Proxy：管控国外的流量；🌍 Direct - 直连，不可访问外网；代理服务器 - 可访问外网

    🔰 Proxy：管控国内的流量；🌍 Direct - 智能分流 (Pac)；☁️ Proxy - 全局代理

    🍎 Proxy： 管控苹果的流量；如果苹果某些服务直连困难，设其为代理，可能会改善一些问题：🍎 Proxy - 代理服务器

    建议 ： ☁️ Proxy - 代理服务器；🔰 Proxy - 🌍 Direct ；🍎 Proxy - 🌍 Direct/代理服务器


#### 🚀 SSR 混淆模式 https://github.com/breakwa11/shadowsocks-rss/blob/master/ssr.md

    理论上开启混淆模式的时候可以利用混淆做到乱序大小的发送和接收，至少可以在某种程度上可以避开GFW的探测，那就应当会获得更好的速度、稳定性以及安全性。


#### 🔋 Surge for iOS 耗电

    Surge 会接管全局的（几乎）所有通信，所以所有的网络方面电量消耗都会被算在 Surge 头上，实际使用中不会感到 Surge 对电量有明显影响。


#### ☑️ Set as System Proxy

    启用 Surge for Mac 后勾选下拉菜单中的 Set as System Proxy 即可自动向系统网络设置添加必要的参数，因为需要修改系统网络设置，首次勾选时需要输入管理员密码进行确认，去掉 Set as System Proxy 的勾选，会清除网络设置中的代理相关设置。


#### 📶 Surge for iOS 开启共享模式 https://medium.com/@scomper/局域网其他设备共享上网-dd29e18853da#.6w19tdsh9

    Surge 在增加了代理共享模式，只需要开启就能让 Wi-Fi 网络中的其他设备通过这台 iPhone 代理访问网络。
    到高级设置中开启 Allow Wi-Fi Access ，或者直接修改配置文件，添加一行参数 allow-wifi-access = true。

    其他 Wi-Fi 网络环境下的设备可以输入已经开启共享代理的 Surge 设备的 IP 地址和端口号，（技巧：Surge Log 中能看到开启后本机的 IP 地址和监听端口）将 IP 地址填写到需要共享设备的 Wi-Fi 信息的 HTTP 代理里即可。


#### 🏃 Auto / Benchmarik

    测试结果仅供参考，无法检测出 VPS 的带宽

    请不要使用 google.com 作为测试目标，有可能导致 proxy 服务器 ip 被加入黑名单，导致各种操作需要输入验证码。
    目标 URL 对所有的 policy 是基本公平的，所以请选择像 gstatic.com 这样的在全球都有节点的 URL 作为测试目标。
    作者建议：http://www.gstatic.com/generate_204



# more

🔰 客户端（有“R”标示表示支持 SSR）：

    * iOS
    
        Surge：https://appsto.re/cn/D0Q_9.i
        
        Shadowrocket (R)：https://appsto.re/cn/UDjM3.i
        
        Wingy (R)：https://appsto.re/cn/19xBeb.i
        
        Potatso (R)：https://appsto.re/cn/OIk1_.i
        
    * Android
    
        ShadowsocksR (R)：https://github.com/shadowsocksr/shadowsocksr-android/releases
        
        Postern (R)：http://www.tunnel-workshop.com
        
    * macOS
    
        ShadowsocksX：https://github.com/shadowsocks/shadowsocks-iOS/releases

        ShadowsocksX-R (R)：https://github.com/yichengchen/ShadowsocksX-R/releases

        ShadowsocksX-NG (R)：https://github.com/qinyuhang/ShadowsocksX-NG/releases
        
        Flora：https://github.com/huacnlee/flora-kit

        Specht Lite：https://github.com/zhuhaow/SpechtLite/releases
        
        Surge：http://nssurge.com
        
    * Windows
    
        ShadowsocksR (R)：https://github.com/shadowsocksr/shadowsocksr-csharp/releases
        

📋 教程 / 说明：

        Surge for iOS：https://medium.com/@scomper/surge-配置文件-a1533c10e80b#.9fpdjn34f
    
        Surge for macOS：https://medium.com/@scomper/surge-for-mac-简明指南-f6f357b8f09c#.n55zdnvnd
    
        Shadowrocket for iOS：http://matrix.sspai.com/p/c113cba0
    
        SSR for Windows：https://ocvpn.wordpress.com/2016/10/15/shadowsocksr-for-windows设置教程
    
        SSR for Android：https://yhyy135.github.io/how-to-use-ssr-android/
    
        SpechtLite for macOS：http://www.jianshu.com/p/2acfcbfee27f

# License

* 可以拷贝、转发，但是必须提供原作者信息，同时也不能将本项目用于商业用途。
