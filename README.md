# 软件介绍

这是一款基于PySide6的一款打包工具，采用了[Nuitka](https://github.com/Nuitka/Nuitka)作为核心
# v1.0

>使用[联机许可证]

[联机许可证]:http://license.rosmontis.com

使用域名txt解析获取授权状态

使用wmi获取设备信息

# v1.1

>使用脱机临时许可证 ~~(暂时方案)~~

使用ntp在线授时校验脱机许可证有效性

# v1.2

更新GUI，可在GUI内完成授权配置

新增文件/文件夹链接

# v1.3

添加了图标预览

调整了动画效果 `QEasingCurve.InOutQuad` -> `QEasingCurve.InOutBack`

完善了[id.py](id.py)的自动填写，现在授权可以完全用软件控制

# v1.4

将各个tab拆分为单个组件

采用[Fluent Design](https://github.com/zhiyiYo/PyQt-Fluent-Widgets)设计

支持切换python，支持自动检测python

- *当前扫描路径与深度*
```
'C:\\', 2
'C:\Program Files', 3
'C:\Program Files (x86)' 3
'D:\\', 4
'E:\\', 4
```

添加了关于页面

# ~~v2.0 (todo)~~  **分支版本**

>使用脱机临时许可证 ~~(暂时方案)~~

"*使用ntp在线授时校验脱机许可证有效性*"

使用RSA+AES混合加密保存脱机证书

|server||client|
|-|-|-|
|*RSA_Pu*|-->||
||<--|**RSA_Pu(** *AES* **)** + **AES(** *id* **)**
|**AES(** *id+license* **)**|-->||
