# ETK++ - The Easy Toolkit for C++ programing

Copyright (C) 2004-2018 Anthony Lee, All rights reserved.

<br>

+ 大部分构思及实现的灵感来源于曾经辉煌一时的 BeOS API；

+ ETK++ 库为自由软件，可在遵循 MIT 协议下使用及传播。

<br>

# 源代码相关

+ 项目实现与 HaikuOS、Cosmoe 等类似实现不存在任何直接关系；

+ 2008 年以前的旧源代码见 [HaikuArchives/EasyToolkitAndExtension](https://github.com/HaikuArchives/EasyToolkitAndExtension)；

+ 新版本不再开放源代码。

以上所提及 2008 年以前的旧源代码，近期我才发现在 GitHub 上（也许是 OSDrawer.net 管理员好心传了上去）。因部分项目未在遵循 MIT 协议下使用及传播前述旧源码，新版本不再开放源代码。

<br>

# 运行库及扩展件

+ 本项目仅发布 Windows 平台下二进制运行库及扩展件；
+ OpenWrt Linux 平台部分机型可参考 [LBKit](https://github.com/DonAnthonyLee/LBPanel_LBKit/wiki) 项目；
+ 其他平台因依赖关系等因应各发行版变化过于繁复不再提供。

<br>

# 版本变更主要内容

## 0.4.3 <= 0.4.2

* ELooper 类，按 BeBook 完善，即构建函数自锁，Run()后解锁，但 EApplication 除外。
* EMessageQueue 类，部分改进，解决某些情况下 ELooper 退出时的越界访问。
* EMessage 类，头文件 RemoveData() 成员函数参数修正。
* EView 类，修正 MessageReceived()，即默认不予采用 EHandler::MessageReceived()。
* KernelKit 相关，修正此前程序退出无规律死锁的问题（由 etk_port 相关导致）。

