---
title: "新建预算"
date: 2022-01-25T17:48:22+08:00
weight: 10
description: >
    新建预算并配置告警信息
---

### 前提条件

若需配置告警接收人或机器人请先确保以下条件：

- 已[添加接收人]({{< relref "../../../auth_security/notify/tutorial/recipient/create" >}})；
- 已[配置机器人]({{< relref "../../../auth_security/notify/tutorial/bot/create" >}})；

### 操作步骤

该功能用于新建预算并设置告警信息。当用户的使用情况超过阈值时，将会通知并提醒用户。

1. 在左侧导航栏，选择 **_"费用/分析/预算管理"_** 菜单项，进入预算管理页面。
2. 单击列表上方 **_"新建"_** 按钮，进入新建预算管理的页面。
3. 配置预算信息：
    - 应用范围：包括系统、域和项目。
        - 当应用范围选择系统时，即预算全局生效。
        - 当应用范围选择指定域时，即预算在指定域生效。
        - 当应用范围选择指定项目时，即预算在指定项目生效。
    - 名称：设置预算的名称。
    - 预算周期：设置预算重置实际支出和预测支出的频率，选择天表示每天一次，月表示每月一次，年表示每年一次。默认预算周期为月。
    - 开始时间/结束时间：设置预算的生效日期，开始时间和结束时间与预算周期有关。
        - 当预算周期为天时，选择预算生效的开始日期和预算结束的结束日期。
        - 当预算周期为月时，选择预算生效的开启月份和预算结束的结束月份。
        - 当预算周期为年时，选择预算生效的开启年份和预算结束的结束年份。
    - 账单类型：选择预算生效的账单类型，默认可选项为平台中纳管的账单的货币类型。当开启多币种账单合并展示开关后，可选项将会以某种货币类型展示全部账单等。
    - 预算金额：设置在预算周期内的预算金额。
    - 高级配置：单击“高级配置”超连接，展开高级配置选项，设置预算的条件等。
        - 云平台：默认为全部平台，支持指定平台。
        - 云账号：默认为全部云账号，当指定平台时，将会根据平台过滤云账号。
        - 云订阅：默认为全部云订阅，当指定平台和云账号时，将会根据平台和云账号过滤可选的云订阅。
        - 区域：默认为全部区域，当指定平台后，可根据平台支持区域指定具体区域。
        - 资源类型：默认不限资源类型，可根据需求设置指定资源类型。
        - 标签：支持两种标签匹配策略，匹配以下任意标签和匹配以下全部标签，即针对于匹配以下任意标签的资源做预算，或针对于匹配以下全部标签的资源做预算，设置标签匹配策略后，选择具体的标签。
4. 单击 **_"确定"_** 按钮，进入配置告警页面。如不需要配置告警，可单击 **_"跳过"_** 按钮。
5. 如需配置告警，设置以下信息：
    - 告警类型：目前只支持成本预算。
    - 告警阈值：设置触发告警的费用金额。支持在金额旁边设置绝对值和百分比。例如200元的预算，如果您想在160元时接收通知，请选择绝对值输入160元或百分比预算设置80。
    - 告警接收人：设置接收告警消息的接收人。
{{% alert title="说明" %}}
- 管理后台下，可以选择所有接收人；
- 域管理后台下，可以选择所有加入到本域或属于本域的接收人；
- 项目视图下，只能选择当前登录用户。
{{% /alert %}}
    - 通知渠道：设置接收人接收告警消息的通知渠道。当选择多个接收人时，通知渠道取接收人支持的通知渠道的交集。
    - 告警机器人：选择接收告警消息的告警机器人。
5. 单击 **_"确定"_** 按钮，完成操作。