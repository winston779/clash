
# clash for windows使用教程

## 下载与安装

* trojan-cdn [下载地址](https://repo.trojan-cdn.com/clash_for_windows_pkg/LatestRelease/) 
    * Windows 请下载 Clash.for.Windows.Setup.[版本号].exe ，一般不要下载带 arm64 的 exe 文件
    * macOS 请下载 Clash.for.Windows-[版本号].dmg 
* github [下载地址]https://github.com/Fndroid/clash_for_windows_pkg/releases

> M1 / M2 macOS 安装时出错请查看常见问题

> Windows 直接双击打开 exe 文件进行安装，如果提示 阻止了无法识别的应用启动。 请点击更多信息，然后再点击仍要运行进行安装。

## 获取订阅链接

初次使用可以选择免费的机场订阅或者购买推荐机场订阅

* [免费机场订阅](https://github.com/winston779/clash/blob/main/%E5%85%8D%E8%B4%B9clash%E6%9C%BA%E5%9C%BA%E8%AE%A2%E9%98%85%E9%93%BE%E6%8E%A5.md)
* [推荐机场订阅](https://github.com/winston779/clash/blob/main/%E6%9C%80%E6%96%B0clash%E6%9C%BA%E5%9C%BA%E6%8E%A8%E8%8D%90.md)

> 注：订阅链接与您的密码一样重要，请勿分享给他人，如不慎泄露，请在产品详情页面重置链接。

## 添加配置

### 1.Clash 主界面介绍

安装后 Windows 可以通过双击通知区域的 Clash for Windows 图标打开主界面

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/cfw-1.png)

> 首先打开 Profiles 配置选择页面，然后进行配置文件的添加

### 2.通过链接直接添加

复制 获取配置 步骤中得到的订阅 URL，粘贴到 Download from a URL 输入框内，点击右侧的 Download 按钮。

显示 Success! 表示成功添加了配置文件，并且下面会多了一个配置，点击可以切换到对应的配置。 具体使用方法请参考后面教程。

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/cfw-2.png)

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/cfw-3.png)

## Clash 代理使用介绍

### 1.开启系统代理与开机启动

首先打开 General 首页页面, 开启系统代理与开机自动启动，然后打开 Proxies 代理服务器选择页面。

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/cfw-4.png)

点击 Global 标签，确认全局规则选择不是 DIRECT (选择 DIRECT 表示不使用代理) ，可以选择 AUTO（自动选择节点，在 Global 页面最底部）或是直接选择自己想要使用的节点。

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/cfw-5.png)

选择节点后可能没有立即生效，建议返回 General 首页页面 点击 Clash for Windows 字样通过快速重启客户端重新载入配置。

这时 Clash 已通过设置系统代理的方式进行工作，使用系统代理的软件已可以正常使用。

可以使用 IE / EDGE / Safari 访问 https://www.google.com 测试

### 2.Global 全局规则选项

Global 页面是设置 Clash 的代理规则，即设置 Clash 如何处理访问请求。

* Direct 表示直接连接，不使用代理

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/cfw-6.png)

* Reject 表示全部拒绝访问

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/cfw-7.png)

* 其他直接选中节点表示全部请求均通过代理，类似于 Shadowsocks 的全局模式
* 选择 Global 右侧的 Rule 标签，表示使用的是自动切换模式，与其他软件的 PAC 模式类似

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/cfw-8.png)

一般完成以上设置后开启客户端的 System proxy 即可正常访问 https://www.google.com ，如果开启后无法使用(软件冲突或是安全软件限制导致客户端无法修改系统设置)，请查看后面部分安装浏览器扩展使用。

## Chrome / Edge / Firefox 配合 SwitchyOmega 扩展

如果不使用客户端的系统代理，可以参考下面教程通过安装浏览器扩展使用（支持 Chrome / Firefox / 新版 Edge 浏览器）

设置方法请参考：Chrome / Edge / Firefox 安装 Proxy SwitchyOmega 扩展使用

由于扩展中代理模式对应客户端的端口为 1080，需要修改为 Clash 对应的 7890，请按照下图进行修改：

![image](https://raw.githubusercontent.com/winston779/clash/main/imgs/cfw-9.png)

## 常见问题

1. 如果您下载的是 Clash for Windows ARM64 版本，打开时如果出现 提示损坏，无法打开 的情况
 
请打开终端程序(在您的 macOS 启动台中搜索终端或是 Terminal )，复制粘贴下面的命令
 
```
sudo xattr -r -d com.apple.quarantine /Applications/Clash\ for\ Windows.app
```
回车执行，输入您的账户密码后，再打开试试
 
2. 如果您下载的不是 ARM64 的版本，打开时提示 无法验证开发者 ，请右键客户端图标，再选择打。
