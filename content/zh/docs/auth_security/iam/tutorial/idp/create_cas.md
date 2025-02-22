---
title: "新建CAS认证源"
date: 2021-12-06T15:34:48+08:00
weight: 20
edition: ee
description: >
    新建CAS认证源
---

1. 在左侧导航栏，选择 **_"认证与安全/认证体系/认证源"_** 菜单项，进入认证源页面。
2. 单击列表上方 **_"新建"_** 按钮，进入新建认证源页面。
2. 配置以下参数：
    - 认证源归属：设置认证源的归属范围，当认证源归属于系统时，即系统中所有用户都可以使用该认证源登录平台。当认证源归属于域时，只有该域中的用户可以使用该认证源登录平台。域管理后台下，认证源归属于域管理员所属域。
    - 名称：设置认证源的名称。
    - 备注：设置认证源的备注信息。
    - 认证协议：选择“CAS”。
    - 认证类型：支持通用CAS。
    - CAS服务地址：CAS单点登录服务器的URL地址，如[http://cas.example.io/cas](http://cas.example.io/cas)。
    - 用户ID：设置通用CAS中对应的用户ID属性，一般为cas:user，如有变化请更改该项。
    - 用户名：设置通用CAS中对应的用户名属性，一般为cas:user，如有变化请更改该项。
    - 自动创建用户：勾选自动创建用户后，通过认证源首次登录的用户将会自动在系统中创建一个本地用户。不勾选该项时，该认证源作为辅助认证源，需要将用户关联到该认证源，才可以通过该认证源登录平台。
    - 用户归属目标域：勾选自动创建用户后才需要设置该参数。选择通过该认证方式登录自动创建的用户所属的域，当认证源归属于域时，用户归属目标域与认证源归属域一致，不可更改。
         
    **高级配置**：默认隐藏，可根据需求进行配置。

    - 默认项目：设置通过CAS认证源登录并在平台自动创建的用户加入的默认项目，当选择“优先使用CAS中的项目”时，需要指定加入项目的字段名，如cas:proj等。用户通过CAS登录时会带有项目字段，若云管平台有匹配的项目，则直接将用户加入到对应项目，如没有匹配的项目，则自动创建同名项目。
    - 默认角色：设置通过CAS认证源登录并在平台自动创建的用户加入项目的默认角色，当选择“优先使用CAS中的角色”时，需要指定角色的字段名，如cas:role等。用户通过CAS登录时会带有角色字段名，若云管平台有匹配的角色，则直接使用对应的角色加入项目。如没有匹配的角色，则使用默认角色加入项目。
    - 显示名：设置通用CAS中对应的显示名字段。
    - 邮箱：设置通用CAS中对应的邮箱字段。
    - 手机号：设置通用CAS中对应的手机号字段。
3. 单击 **_"确定"_** 按钮，连接认证源，并同步认证源上的域、组和用户信息。
