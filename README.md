# Loon4Mac
Loon for Mac

# 邀请测试阶段
Loon已经完成了部分用户内测阶段，完成了基本的功能，但由于目前很多UI功能不够完善、BUG比较多，为了避免在使用过程中遇到异常影响正常的工作和生活，目前Loon for Mac暂时只接受申请测试的用户使用。

## 申请测试方式
更新到iOS端Loon 3.3.3(890)版本及以上版本，在Loon for Mac中获取测试码。

# Bug反馈

## 自动反馈
Loon集成了Firebase的Crash收集SDK，仅仅用来获取崩溃日志，便于bug修复，由于一些分流规则会拦截此类请求，所以希望尽可能禁用这些规则，但是Loon不会强制放行这些请求，请放心使用。后续版本稳定后会给出是否自动发送Crash的选项。

## 手动提交
如果遇到阻塞问题或者其他用户体验问题：
- 可以直接在本仓库提交issue
- 可以在Loon的[Telegram社区群](https://t.me/Loon0x00)提交

# 隐私说明

## 目前版本的Loon for Mac所需的权限
### 系统网络扩展
Loon使用的是macOS System Extension，该扩展运行在系统内核栈，所以需要运行Loon使用系统扩展才可以启动Network Extension。在第一次启动VPN是会出现如下图所示的提示，这是需要**点击打开系统设置**进入系统设置页面运行Loon使用扩展即可。如果后续无法出现弹框，可在**系统设置-登录项-扩展-网络扩展**中找到。
![System Extension](/Resource/sys_extension.jpg)
![Network Extension](/Resource/network_extension.png)

### 访问本地网络权限
用于局域网访问。

### 定位权限
从macOS10.15开始，苹果加强了对于获取WiFi的SSID等信息获取限制，必须要获取定位权限才能获取WiFi的SSID，为了SSID策略组的正常使用需要此项权限，我们**绝对不会获取您的定位信息，更加不会上传到任何服务器**，请放心授权。如果实在不放心，或者没有用到SSID策略组，那也可以不允许这个选项。

### 通知权限
发出Loon相关的通知，此项和iOS相同。