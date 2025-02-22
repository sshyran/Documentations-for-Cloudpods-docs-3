---
title: "设置读写权限"
date: 2021-11-26T16:50:33+08:00
weight: 40
description: >
    设置存储桶的读写权限
---

该功能用于设置存储桶的读写权限。

{{% alert title="说明" %}}
- 腾讯云存储桶不支持公开读写；
- Azure存储桶不支持认证用户可读和公开读写；
- AWS存储桶不支持超认证用户可读、本账号写公开读和公开读写；
- 阿里云、Ceph存储桶不支持认证用户可读；
- 阿里金融云内网区域的存储桶不支持设置读写权限的操作。
{{% /alert %}}

1. 在左侧导航栏，选择 **_"存储/对象存储/存储桶"_** 菜单项，进入存储桶页面。
2. 单击存储桶右侧操作列的 **_"更多"_** 按钮，选择 **_"设置读写权限"_** 菜单项，弹出设置访问权限设置对话框。
2. 设置读写权限：包括本账号读写、本账号公开读、公开读写。
    - 本账号读写：只有用户本人可以读写指定存储桶中的数据。
    - 认证用户可读：已认证用户可读取bucket中的数据，仅用户本人可执行写操作。
    - 本账号写公开读：任何用户均可读取存储桶中的数据，但是向存储桶写数据需要进行身份验证。
    - 公开读写：任何用户均可读写存储桶中的数据，无需身份验证，该权限安全风险极高，为保证您的数据安全，请谨慎选择。
3. 单击 **_"确定"_** 按钮，完成操作。