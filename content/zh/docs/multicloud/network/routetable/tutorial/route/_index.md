---
title: "管理路由"
date: 2022-01-04T14:15:00+08:00
weight: 20
description: >
    管理路由表下的路由
---

路由表通过路由来实现流量走向控制，路由是由目标网段、下一跳类型和下一跳组成：

- 目标网段：即流量将要转发的目的地址，为网段格式。
- 下一跳类型：VPC的数据包的出口。VPC下一跳类型支持 “NAT 网关”、“对等连接”、“虚拟机”等类型。
- 下一跳：指流量将要跳转的实例，可以是具体的虚拟机、NAT网关实例等。


