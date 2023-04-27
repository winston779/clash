# Shadowrocket苹果ios使用教程

## 1.购买Shadowrocket代理服务

* [2023机场推荐](https://github.com/winston779/clash/blob/main/%E6%9C%80%E6%96%B0clash%E6%9C%BA%E5%9C%BA%E6%8E%A8%E8%8D%90.md)
* [免费机场推荐](https://github.com/winston779/clash/blob/main/%E5%85%8D%E8%B4%B9clash%E6%9C%BA%E5%9C%BA%E8%AE%A2%E9%98%85%E9%93%BE%E6%8E%A5.md)

## 2.获取外区苹果 id

国内商店无 VPN 相关 APP，因此需要使用外区 Apple id 登录 App Store 才可下载 Shadowrocket。 而且需要绑定外区支付方式，这个过程其实是相对麻烦的。我们推荐直接 bing 搜索[ 小火箭 Shadowrocket ]。购买外区已购 Shadowrocket 的成品账号下载软件。

## 3.在 App Store 登录外区苹果 id

> 必须在 App Store 中切换苹果 id，请勿在系统设置中登录外区 id，可能泄漏隐私，可能导致手机锁定

点击 App Store → 点击右上角头像 → 滑到页面底部，点击 退出登录 → 然后回到页面顶部，登录准备好的外区苹果 id

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/shadowrocket-1.jpeg)

## 4.下载 Shadowrocket 

确认已经切换账号后， 点击下载 [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118) 。或者扫码下载，安装 APP。

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/shadowrocket-2.jpeg)

>如果提示 App 不可用，重启 App Stroe，检查下 苹果 id 是否切换成功

## 5.通过订阅链接导入

打开 Shadowrocket，点击底部导航栏的「设置」进入设置页面，随后往下划至最底部，进入「服务器订阅」子页面。

将「打开时更新」的开关 打开。

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/shadowrocket-3.jpeg)

回到首页，点击右上角的加号，再次点击第一行的「类型」，选择 Subscribe。

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/shadowrocket-4.jpeg)

在「备注」中输入: 名称 ，随后在「URL」中粘贴上方机场中的订阅链接并保存。

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/shadowrocket-5.jpeg)

随后点击右上角保存，此时会自动更新获取服务器。

## 6.更新订阅更新节点

> 提示：机场节点信息可能会不定时更新，若出现大面积节点不可用现象，请手工更新订阅。

在主界面，点击订阅右侧的 刷新 按钮即可，如下图：

![image](https://w1.v2free.top/docs/SSPanel/iOS/images/shadowrocket-6.jpg)

更新节点注意事项：如果开启VPN，确保选择可用的节点，如果当前没有可用节点，先关闭vpn再更新。

## 7.分流规则

小火箭自带的一个简单的默认配置，有基本分流功能，自带规则比较精简，包含了常用网站，好处是体积小速度快，缺点是你上的网站如果不是常用或者是个cdn，它不一定会走代理。如果你不满意，可以继续下载配置一个高级分流规则。

在底部导航栏进入「配置」页面，点击右上角加号。

在弹出的输入框中输入 [此链接网址](https://w1.v2free.top/Shadowrocket.conf) 【电脑：右键点链接->复制链接地址；手机长按链接，然后复制链接地址；或点击打开链接后从浏览器地址栏复制链接地址】。

随后点击 远程文件 中新增的配置文件地址，在弹出的菜单中选择第二个「使用配置」，此时 APP 会自动开始下载配置并应用配置。
