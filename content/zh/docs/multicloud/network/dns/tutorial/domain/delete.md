---
title: "删除域名"
date: 2021-11-25T16:05:25+08:00
weight: 60
description: >
    删除DNS解析域名
---

该功能用于删除DNS解析域名，支持单个和批量操作。

**单个删除**

1. 在左侧导航栏，选择 **_"网络/网络服务/DNS解析"_** 菜单项，进入DNS解析页面。
2. 单击域名右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"删除"_** 菜单项，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。

**批量删除**

1. 在DNS解析列表中选择一个或多个域名，单击列表上方 **_"删除"_** 按钮，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。

```
# 删除DNS解析域名
$ climc dns-zone-delete <DNS解析域名ID或名称> 
```