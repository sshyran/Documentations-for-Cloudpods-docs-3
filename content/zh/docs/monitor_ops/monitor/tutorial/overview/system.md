---
title: "查看系统总览"
date: 2022-01-17T19:28:27+08:00
weight: 10
description: >
    查看系统总览信息
---

在系统视图下支持查看以下指标：

- 资源概览：
    - 虚拟机：显示系统中虚拟机的总数量，以及发生告警、正常状态、未设置告警的虚拟机数量及百分比。
    - 宿主机：显示系统中宿主机的总数量，以及发生告警、正常状态、未设置告警的宿主机数量及百分比。
    - 云账号：显示系统中云账号的总数量，以及发生告警、正常状态、未设置告警的云账号数量及百分比。    
    - 对象存储：显示系统中对象存储的总数量，以及发生告警、正常状态、未设置告警的对象存储数量及百分比。
    - RDS：显示系统中RDS的总数量，以及发生告警、正常状态、未设置告警的RDS数量及百分比。
    - Redis：显示系统中Redis的总数量，以及发生告警、正常状态、未设置告警的Redis数量及百分比。
    - 存储：显示系统中块存储的总数量，以及发生告警、正常状态、未设置告警的块存储数量及百分比。
- 未恢复告警：显示系统中所有未恢复告警的数量，支持以环形图的形式展示未恢复告警的总数量以及不同资源类型的告警数量。点击将会跳转到告警历史 - 未恢复告警页面。
- 近30天告警趋势：支持以折线图或堆叠柱状图的形式展示系统中近30天的告警数量、不同资源类型的告警数量、占告警总数的比例以及告警趋势。通过单击右上角![](../../../images/switch.png)图标来切换趋势图的展示形式。
- 支持查看系统指标。
    - 查看虚拟机近N天中Top N的平均CPU使用率、内存使用率、磁盘使用率、磁盘读速率、磁盘写速率、网络入流量、网络出流量、等指标。其中内存使用率、磁盘使用率指标需要为虚拟机安装监控Agent。
    - 查看宿主机近N天中Top N的平均CPU使用率、磁盘读速率、磁盘写速率、网络入流量、网络出流量、等指标。
    - 默认为虚拟机或宿主机，表示不聚合，可通过系统、域、项目、平台、区域、可用区等维度查看指定维度下的虚拟机或宿主机的指标。
        - 系统：用于查看平台上虚拟机或宿主机的平均使用情况。
        - 域：用于查看不同域下的虚拟机或宿主机的平均使用情况。
        - 项目：用于查看不同项目下的虚拟机的平均使用情况。
        - 平台：用于查看不同平台下的虚拟机或宿主机的平均使用情况。
        - 区域：用于查看不同区域下的虚拟机或宿主机的平均使用情况。
        - 可用区：用于查看不同可用区下的虚拟机或宿主机的平均使用情况。
    - 时间范围包括近1小时、近6小时、近12小时、近1天、近7天、近14天、近一个月，默认为近7天；
    - Top N包括Top10、Top20、全部，默认为Top10。

- 列表用于展示系统下近N天，不同聚合维度下的虚拟机或宿主机的平均CPU使用率、网络入流量、网络出流量、磁盘读速率、磁盘写速率等指标。支持单击表格右上角![](../../../../images/download.png)图标，导出对应的监控数据。