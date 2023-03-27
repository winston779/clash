

# 安卓手机clash for android使用教程

## 1.下载

有几种下载方式，大家选择适合的：

* Google Play商店下载，[点击链接](https://play.google.com/store/apps/details?id=com.github.kr328.clash)
* Github [点击链接](https://github.com/Kr328/ClashForAndroid/releases)，下载最新Latest版本的cfa-[版本号]-foss-universal-release.apk 或 cfa-[版本号]-premium-universal-release.apk （注)
* trojan-cdn [点击链接](https://repo.trojan-cdn.com/ClashForAndroid/LatestRelease/) 下载cfa-[版本号]-foss-universal-release.apk 或 cfa-[版本号]-premium-universal-release.apk
> 注：其中的armeabi-v7a、arm64-v8a、x86 和 x86_64是CPU架构，如果你是安卓模拟器就选择x86_64，真实的安卓手机选择arm64-v8a，如果无法运行再尝试armeabi-v7a安装包，当然选择universal安装包就不需要这样尝试了，因为安装包包含了全平台可执行程序文件，因此安装包也大了近3倍。这里，app后面又有foss和premium两种类型，其中premium表示使用了Clash premium闭源版本(更多功能,但没有源码)。

## 2.获取订阅链接

初次使用可以选择免费的机场订阅或者购买推荐机场订阅

* [免费机场订阅](https://github.com/winston779/clash/blob/main/%E5%85%8D%E8%B4%B9clash%E6%9C%BA%E5%9C%BA%E8%AE%A2%E9%98%85%E9%93%BE%E6%8E%A5.md)
* [推荐机场订阅](https://github.com/winston779/clash/blob/main/%E6%9C%80%E6%96%B0clash%E6%9C%BA%E5%9C%BA%E6%8E%A8%E8%8D%90.md)

> 注：订阅链接与您的密码一样重要，请勿分享给他人，如不慎泄露，请在产品详情页面重置链接。

## 3.添加节点(通过订阅链接)

安装后打开首页，点击配置：

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/clash_for_android_1.jpg)

点击新配置：

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/clash_for_android_2.jpg)

点击 URL (从 URL 导入)：

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/clash_for_android_3.jpg)

粘贴 Clash 订阅链接，点击右上角的保存：

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/clash_for_android_4.jpg)

下载完成后选中配置文件，然后返回首页点击 点此启动 开始使用：

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/clash_for_android_5.jpg)

第一次启动时会请求 VPN 权限，需要点击确定允许。

(该弹窗为系统弹窗，与客户端无关，如果无法点击基本上是其他 APP 有在使用悬浮窗权限导致，或者是一些系统的护眼模式)

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/clash_for_android_6.jpg)

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/clash_for_android_7.jpg)

如果需要切换节点，请点开第二个 代理 选项即可。

切换代理模式的方法：

点击 设置 > 覆写 > 代理模式。

## 4.日常使用问题

* 日常某些可能不可访问，可以选择自动，这样会优先访问延迟较低的节点。
* 订阅链接默认选择自动更新，由于机场会不定期修改端口、IP等操作，发现大部分节点不能访问时，可以选择手动更新订阅。
