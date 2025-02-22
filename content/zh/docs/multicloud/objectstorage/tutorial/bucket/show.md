---
title: "查看存储桶详情"
date: 2021-11-26T16:52:59+08:00
weight: 70
description: >
    查看存储桶详情页
---

该功能用于查看存储桶的详细信息。

1. 在左侧导航栏，选择 **_"存储/对象存储/存储桶"_** 菜单项，进入存储桶页面。
2. 单击指定存储桶名称项，进入文件列表页面。
2. 单击“详情”页签，进入存储桶详情页面。
3. 查看以下信息
    - 基本信息：包括存储桶的云上ID、ID、名称、状态、域、项目、共享范围、平台、区域、位置（可用于查看阿里金融云存储桶是否为内网区域）、存储类型、可用区、云账号、创建时间、更新时间、备注等。
    - 访问域名：创建存储桶后会生成对应的访问域名以及S3网关，用户可通过S3网关统一管理存储桶等。
    - CDN加速域名：显示存储桶设置的CDN加速域名。
    - 静态网站：显示存储桶静态网站的访问链接等。
    - 用量统计：存储桶已使用容量统计。包括存储用量以及文件数量。
    - 用量上限：存储桶设置的容量上限。包括存储容量上限和文件数量上限。
    - 访问权限：设置存储桶的访问权限，包括本账号读写、本账号公开读、公开读写，本账号的信息可通过查看存储桶的后端访问信息获取。
        - 本账号读写：只有用户本人可以读写指定存储桶中的数据。
        - 认证用户可读：已认证用户可读取bucket中的数据，仅用户本人可执行写操作。
        - 本账号公开读：任何用户均可读取存储桶中的数据，但是向存储桶写数据需要进行身份验证。
        - 公开读写：任何用户均可读写存储桶中的数据，无需身份验证，该权限安全风险极高，为保证您的数据安全，请谨慎选择。
    - 防盗链：显示存储桶是否设置了防盗链。


