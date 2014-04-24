---
layout: wiki
title: 介绍几个常用的宏的作用
---

# {{ page.title }}

## ENABLE_UART
启用串口打印功能。要想调试期间把信息打印到串口，还需要加上宏：DEBUG_PRINT_ON_UART 

## USE_UART_CRTP
crtp模块为：Crazy Realtime Transfer Protocol stack，是crazy flie的通信协议栈。通信链路可以2.4G 遥控信息，可以使用USE_ESKYLINK，也可以使用串口。若要使用蓝牙模块作为通信链路，应该开启此宏。

## DEBUG_PRINT_ON_UART
使用串口调试。在平衡算法当中进行调试的时候，串口打印显得尤为重要，通过此宏可以开启串口调试。注意：开启串口调试的时候不能开启宏USE_UART_CRTP，串口作为通信链接。

## BOARD_2
此宏在drivers/i2c_gpio.c文件中。因为版本2与版本3的i2c部分引脚有区别，去掉此宏定义适用于第三版的硬件

