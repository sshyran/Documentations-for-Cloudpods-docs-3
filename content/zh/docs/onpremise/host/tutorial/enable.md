---
title: "启用/禁用"
date: 2022-02-07T18:24:26+08:00
weight: 30
description: >
    控制宿主机的启用状态，启用状态下的宿主机用于创建虚拟机
---



### 启用

该功能用于启用"禁用"状态的宿主机。启用状态的宿主机用于创建虚拟机。

<big>**界面操作**</big>

**单个启用**

1. 在左侧导航栏，选择 **_"主机/基础资源/宿主机"_** 菜单项，进入宿主机页面。
2. 单击"禁用"状态的宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"启用"_** 菜单项，弹出操作确认对话框。
3. 单击 **_"确定"_** 按钮，启用宿主机。

**批量启用**

1. 在左侧导航栏，选择 **_"主机/基础资源/宿主机"_** 菜单项，进入宿主机页面。
2. 在宿主机列表中勾选一个或多个"禁用"状态的宿主机，单击列表上方 **_"启用"_** 按钮，弹出操作确认对话框。
3. 单击 **_"确定"_** 按钮，启用宿主机。

<big>**climc操作**</big>

```bash
# 找到禁用的宿主机
$ climc host-list --disabled

# 启用宿主机
$ climc host-enable <host_id>
```


### 禁用

该功能用于禁用”启用“状态的宿主机，禁用状态的宿主机不能创建虚拟机。

<big>**界面操作**</big>

**单个禁用**

1. 在左侧导航栏，选择 **_"主机/基础资源/宿主机"_** 菜单项，进入宿主机页面。
2. 单击”启用“状态的宿主机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"禁用"_** 菜单项，弹出操作确认对话框。
3. 单击 **_"确定"_** 按钮，禁用宿主机。

**批量禁用**

1. 在左侧导航栏，选择 **_"主机/基础资源/宿主机"_** 菜单项，进入宿主机页面。
2. 在宿主机列表中勾选一个或多个"启用"状态的宿主机，单击列表上方 **_"禁用"_** 按钮，弹出操作确认对话框。
3. 单击 **_"确定"_** 按钮，禁用宿主机。

<big>**climc操作**</big>

```bash
# 禁用宿主机
$ climc host-disable <host_id>
```