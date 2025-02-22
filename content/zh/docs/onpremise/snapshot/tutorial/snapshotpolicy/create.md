---
title: "新建自动快照策略"
date: 2021-12-29T19:35:15+08:00
weight: 10
description: >
    新建自动快照策略，当策略关联公有云平台上的硬盘时将会同步到公有云平台
---

该功能用于创建自动快照策略。云管平台上创建的自动快照策略当关联阿里云或腾讯云平台上的硬盘时，自动快照策略将会同步到阿里云或腾讯云平台上。

1. 单击列表上方 **_"新建"_** 按钮，弹出新建策略对话框。
2. 设置以下参数：
    - 策略名称：设置自动快照策略的名称。
    - 备份日期：选择设置备份的日期，在星期一至星期日之间选择一个或多个日期。
    - 备份时间：选择设置备份的时间点，在00：00至23：00之间选择一个或多个时间点。由于创建快照会暂时降低存储IO性能，出现短暂瞬间变慢的情况，建议备份时间点避开业务高峰时间。
    - 保留时间：包括自定义保留时长和永久保留。
        - 自定义保留时长：超过保留天数后将会自动删除快照，默认保留7天，支持更改自定义设置保留时长，保留天数范围为1-49天。
        - 永久保留：若设置为永久保留，则不删除快照。然而当自动快照超出配额后，{{<oem_name>}}平台上将会自动删除最早创建的自动快照，腾讯云平台上的自动快照策略将不生效。
3. 单击 **_"确定"_** 按钮，创建自动快照。