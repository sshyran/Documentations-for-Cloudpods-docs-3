---
title: "新建定时任务"
date: 2022-01-11T16:22:42+08:00
weight: 10
description: >
    新建定时任务
---

1. 在左侧导航栏，选择 **_"运维工具/常用工具/定时任务"_** 菜单项，进入定时任务页面。
2. 单击列表上方 **_"新建"_** 按钮，进入新建定时任务也没。
2. 配置以下参数：
    - 指定项目：管理员和域管理员在新建定时任务时需要指定定时任务所属的项目。
    - 名称：设置定时任务的名称。
    - 备注：设置定时任务的备注信息。
    - 触发频率：支持选择单次、每天、每周、每月。
        - 当选择“单次”时，设置具体的触发时间。
        - 当选择“每天”时，设置每天具体的触发时间，并设置有效时间。定时任务在有效时间内生效。
        - 当选择“每周”时，选择具体触发星期、触发时间，并设置有效时间。定时任务在有效时间内生效。
        - 当选择“每月”时，选择具体的触发日期、触发时间，并设置有效时间。定时任务在有效时间内生效。
    - 资源类型：目前仅支持虚拟机。
    - 操作动作：目前仅支持开机、关机、重启。
    - 指定虚拟机：选择执行定时任务的虚拟机。单击输入框，在弹出的对话框中选择虚拟机，选择完成后，单击 **_"选择"_** 按钮。
3. 单击 **_"确定"_** 按钮，创建定时任务。