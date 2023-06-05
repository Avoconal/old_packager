![Avoconal](https://github.com/abcdesteve/packager/assets/72078508/6de5d452-b74f-49d5-8ec3-53d1455e6e03)

# 软件介绍
这是一款基于PySide6的一款打包工具，采用了[Nuitka](https://github.com/Nuitka/Nuitka)作为核心

请注意！！！**授权部分尚未开源**
请不要提交有关issue

- ![image](https://github.com/abcdesteve/packager/assets/72078508/6f82957c-8b4b-4290-8ce0-c01d1acc7170)
- ![image](https://github.com/abcdesteve/packager/assets/72078508/07e186a1-6971-4765-b51d-5678f8ea44ec)
- ![image](https://github.com/abcdesteve/packager/assets/72078508/de2b7ef3-4ca1-4ba3-b5a1-e823e3d02a26)
- ![image](https://github.com/abcdesteve/packager/assets/72078508/27261d42-02af-4b67-96f8-0a5d4c699a6e)

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
