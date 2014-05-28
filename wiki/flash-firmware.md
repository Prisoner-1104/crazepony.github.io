---
layout: wiki
title: 主控固件烧写
---

# {{ page.title }}

编译好STM32的代码，得到hex格式的固件文件，如何烧写到主控中？

解压开发工具压缩文件。

把cp2102的驱动装上。这个驱动在32位windows xp系统下测试通过。

![](/assets/img/cp2102.jpg)

打开那个下载器，然后用这个下载器下载hex文件。

![](/assets/img/download.jpg)

下载成功的标注。

![](/assets/img/download-done.jpg)

然后连上usb线，打开压缩包的里的串口助手，波特率115200，看调试参数。

![](/assets/img/uart-info.jpg)