# Aladdin Smart Debugger

![Build with Gradle](https://github.com/5Nut-Inc/aladdin-debugger/workflows/Build%20with%20Gradle/badge.svg)
![Build with Gradle](https://github.com/5Nut-Inc/aladdin-debugger/workflows/Build%20with%20Gradle/badge.svg?branch=master)


## [Why] / 介绍  
Aladdin Smart Debugger 产品的目的帮助Android开发者快速检测、定位产生bug/exception的位置。  
开发者在debug 过程中可视化的显示开发者的操作记录和屏幕状态变化，通过关联操作步骤与代码，快速定位到导致bug的操作相关代码，提高debug的效率。
通过操作步骤的复现，将记录的操作回放到目标程序上，以便于重现bug或检测错误。  

智能debugger的工程原理是：通过代码插桩技术，监听app的操作动作，并通过Android Debug Bridge(ADB) 传输数据到IDE（Android Studio, VS Code, cli 等）上。

* 注: 目前仅开发了Android Studio 插件(aladdin-idea-plugin)和cli(aladdin-cli) ,其它IDE会在以后开发。 (Feb 6, 2020)

## [What.1] 都能干啥
1. [操作步骤复现](#feature-1-操作步骤复现)
2. [错误定位](#feature-2-错误定位)
3. [代码修复建议](#feature-3-代码修复建议)
4. [dump memory heap](#feature-4-dump-memory-heap)

### Feature 1. 操作步骤复现
1. 记录App操作
2. 记录屏幕变化


### Feature 2. 错误定位
1. logcat关联操作步骤
1. 操作步骤关联断点
2. 操作步骤关联屏幕截图
