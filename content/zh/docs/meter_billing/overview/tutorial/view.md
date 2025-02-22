---
title: "查看费用总览"
date: 2022-01-27T11:41:26+08:00
weight: 10
description: >
    查看费用总览页面的相关指标内容
---

1. 在左侧导航栏，选择 **_"费用/总览"_** 菜单项，进入费用总览页面。

**时间控件**：通过切换时间控件查看指定时间范围内的费用总览信息。

默认查看本月的费用信息，支持支持查看本月、上月、本季度、上季度、本年或自定义时间内<img src="../../images/bill/month1.png" width="400" alt="date">费用、消费趋势以及不同维度下的消费占比。

**指标**：查看时间范围内的消费金额、消费趋势及不同维度的消费占比。

- 本月消费：查看平台本月内的消费金额，较上月同期的趋势比值，随时间控件变动，显示对应月份的消费金额，仅本月消费时支持较上月同期的趋势比值分析。
- 本年消费：查看平台本年内的消费金额，随时间控件变动，显示为当前所选日期截止日期的当年费用。

{{% alert title="说明" %}}
账单中出现负数是因为产生了退款，如包年包月机器提前释放退款、使用优惠券后退款、以及账号享受的其他优惠的退款。
{{% /alert %}}

- 消费趋势：以柱状图或折线图的形式展示指定时间范围内的消费金额、消费趋势及预测费用。
{{% alert title="说明" %}}
目前只有本月和本年的消费趋势支持预测费用数据。

- 本月：当存在30天以上的历史账单数据时，可以预测本月剩余时间的所有预测费用，若存在的历史账单数据不足30天，可以预测已出的历史账单一半时间的预测费用。
- 本年：当存在一年以上的历史账单数据时，可以预测本年剩余时间的所有预测费用，若存在的历史账单数据不足一年，可以预测已出的历史账单一半时间的预测费用。
{{% /alert %}}

- 维度分析：支持查看指定范围内不同平台、资源类型、资源、云账号、云订阅、区域、计费模式、域（部门）、项目、标签、自定义维度的消费金额和占总消费数的比例。
    - 平台：以列表的形式显示云管平台上不同平台消费金额及比例，以环形图的形式显示消费总费用和不同平台的消费金额及比例。
    - 资源类型：以列表的形式显示云管平台上不同资源类型（虚拟机和云硬盘）的消费金额及比例；以环形图的形式显示云管平台消费总费用和不同资源类型的消费金额及比例。
    - 资源：以柱形图和列表的形式显示云管平台上消费TOP N(默认为TOP 10，支持修改为TOP 10、TOP 20、TOP 30、全部)的计算资源和消费金额，支持通过资源类型过滤指定资源类型的消费TOP N的计算资源和消费金额，支持通过资源类型过滤指定资源类型的消费TOP N(默认为TOP 10，支持修改为TOP 10、TOP 20、TOP 30、全部)的计算资源和消费金额。柱形图仅包括资源名称和消费金额，列表包括资源名称、资源类型、项目以及费用信息。支持单击右上角![](../../../images/download.png)图标导出对应的账单数据。
    - 云账号：以柱形图和列表的形式显示云管平台上消费TOP N(默认为TOP 10，支持修改为TOP 10、TOP 20、TOP 30、全部)的云账号消费金额。支持单击右上角![](../../../images/download.png)图标导出对应的账单数据。
    - 云订阅：以柱形图和列表的形式显示云管平台上消费TOP N(默认为TOP 10，支持修改为TOP 10、TOP 20、TOP 30、全部)的云订阅消费金额。支持单击右上角![](../../../images/download.png)图标导出对应的账单数据。
    - 区域：以列表的形式显示云管平台在不同区域下的消费金额及比例；以环形图的形式显示云管平台消费总费用和不同区域下的消费金额及比例。
    - 计费模式：以列表的形式显示云管平台上按量付费和包年包月类型计费模式消费的金额及比例；以环形图的形式显示云管平台消费总金额、不同计费模式消费金额及比例。
    - 域（部门）：以列表的形式显示云账号上不同域（部门）的消费金额及比例；以环形图的形式显示云账号消费总费用和不同域（部门）的消费金额及比例。项目视图下不可见。
    - 项目：单击 **_"项目"_** 按钮，在弹出的对话框中选择域，如不填，则代表统计所有域下的项目。以柱形图和列表的形式显示指定域或平台上消费TOP N(默认为TOP 10，支持修改为TOP 10、TOP 20、TOP 30、全部)的项目名称和消费金额。支持单击右上角![](../../../images/download.png)图标导出对应的账单数据。
    - 标签：单击 **_"标签"_** 按钮，在弹出的输入框中选择标签，以列表的形式查看指定标签下的不同标签值对应的资源消费金额及比例；以环形图的形式查看指定标签下的消费总金额、不同标签值对应资源消费金额及比例。

        ![](../../../images/label1.png)
    - 自定义：单击 **_"自定义"_** 按钮，在弹出的输入框中选择自定义维度，以列表的形式查看指定维度下的不同维度项对应的资源消费金额及比例；以环形图的形式查看指定维度下的消费总金额、不同维度值对应的消费金额及比例。