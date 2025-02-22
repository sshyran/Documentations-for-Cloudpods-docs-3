---
title: "关机"
date: 2022-01-06T16:13:23+08:00
weight: 30
description: >
    将处于运行中状态的虚拟机关机
---

该功能用于将处于运行中状态的虚拟机关机。批量关机操作支持选择不同平台上“运行中”状态的虚拟机。

{{% alert title="注意" color="warning" %}}
目前仅阿里云、腾讯云按量付费的虚拟机支持关机不收费。

- 关机后，将释放CPU、内存，并停止对CPU、内存的计费，所关联硬盘、镜像、公网带宽(如需计费)依然计费
- 关机后，实例的 CPU 、内存将不再保留，所以再次启动实例时可能会失败。此时，您可以尝试再次启动，或者换一个时间再次启动
- 关机后，普通公网 IP 将被释放不可找回，建议您先转换为弹性公网 IP 后再进行关机操作
- 关机后，弹性公网 IP 将被保留，不会被释放，关机期间也不收取费用
- 关机期间实例较多操作（如调整配置、重装系统等）可能无法支持，如需操作请开机后进行
- 部分不支持关机不收费的实例，关机后继续正常收费
{{% /alert %}}

**单个虚拟机关机**

1. 在左侧导航栏，选择 **_"主机/主机/虚拟机"_** 菜单项，进入虚拟机页面。
2. 单击“运行中”状态的虚拟机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"实例状态-关机"_** 菜单项，弹出操作确认对话框。
2. 当虚拟机是阿里云或腾讯云平台上按量付费的虚拟机时，可以选择勾选“关机不收费”。
3. 单击 **_"确定"_** 按钮，完成操作。

**批量关机**

1. 在虚拟机列表中选择一个或多个“运行中”状态的虚拟机，单击列表上方 **_"关机"_** 按钮，弹出操作确认对话框。
2. 当被选择的虚拟机是阿里云或腾讯云平台上按量付费的虚拟机时，可以选择勾选“关机不收费”。
3. 单击 **_"确定"_** 按钮，完成操作。 