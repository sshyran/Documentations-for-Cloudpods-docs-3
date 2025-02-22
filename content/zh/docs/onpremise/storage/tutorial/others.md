---
title: "管理块存储"
weight: 7
description: >
  介绍块存储的常用管理操作。
---

## 启用

该功能用于启用"禁用"状态的块存储，禁用状态的存储无法提供存储服务。

**单个启用**

1. 在左侧导航栏，选择 **_"存储/块存储/块存储"_** 菜单项，进入块存储页面。
2. 单击"禁用"状态的块存储右侧操作列 **_"启用"_** 按钮，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，启用存储。

**批量启用**

1. 在存储列表中勾选一个或多个"禁用"状态的存储，单击列表上方 **_"启用"_** 按钮，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，启用存储。

## 禁用

该功能用于禁用”启用“状态的块存储。

**单个禁用**

1. 在左侧导航栏，选择 **_"存储/块存储/块存储"_** 菜单项，进入块存储页面。
2. 单击”启用“状态的块存储右侧操作列 **_"禁用"_** 按钮，禁用存储。

**批量禁用**

1. 在存储列表中勾选一个或多个”启用“状态的存储，单击列表上方 **_"禁用"_** 按钮，禁用存储。

## 调整超售比

该功能用于设置存储的超售比。超售即存储提供超过自身拥有的容量大小。存储实际可分配资源为实际资源*超售比。

{{% alert title="说明" %}}
ZStack平台的存储暂不支持调整超售比。
{{% /alert %}}

**单块存储调整超售比**

1. 在左侧导航栏，选择 **_"存储/块存储/块存储"_** 菜单项，进入块存储页面。
2. 单击块存储右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"调整超售比"_** 菜单项，弹出修改属性对话框。
2. 设置超售比，单击 **_"确定"_** 按钮。

**批量调整超售比**

1. 在列表中勾选一个或多个块存储，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"调整超售比"_** 菜单项，弹出修改属性对话框。
2. 分别设置CPU超售比和内存超售比，单击 **_"确定"_** 按钮。

## 调整容量

仅OpenStack平台支持，由于云管平台获取不到OpenStack平台上存储的真正容量，所以云管平台支持设置OpenStack存储容量，请尽量将存储容量设置为存储的真实容量以尽可能的使用存储，避免由于设置的容量超出存储的真实容量而导致磁盘创建失败。

1. 在左侧导航栏，选择 **_"存储/块存储/块存储"_** 菜单项，进入块存储页面。
2. 单击OpenStack平台上指定块存储右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"调整容量"_** 菜单项，弹出调整容量对话框。
2. 设置容量大小，单击 **_"确定"_** 按钮。

## 修改属性

该功能用于调整块存储的参数信息以及超售比。超售比为虚拟容量与实际容量的比值。

1. 在左侧导航栏，选择 **_"存储/块存储/块存储"_** 菜单项，进入块存储页面。
2. 单击指定块存储右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"修改属性"_** 菜单项，弹出修改属性对话框。
2. 支持修改以下参数：
    - 当选择Ceph类型存储时，支持修改Ceph Key（Ceph用户的密钥）、介质类型；
    - 当选择NFS类型存储时，支持修改NFS Host（NFS服务器IP地址）、NFS Shared Dir（NFS的共享目录）、介质类型；
    - 当选择其它类型存储时，仅支持修改介质类型。
3. 单击 **_"确定"_** 按钮。

## 调整调度标签

该功能用于为块存储绑定调度标签，绑定调度标签的块存储将会按照调度标签为虚拟机提供存储。

1. 在左侧导航栏，选择 **_"存储/块存储/块存储"_** 菜单项，进入块存储页面。
2. 单击指定块存储右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"调整调度标签"_** 菜单项，弹出调整调度标签对话框。
2. 选择调度标签，单击 **_"确定"_** 按钮。

## 更改域

该功能用于更改块存储的所属域。

{{% alert title="说明" %}}
更改域的条件：需同时满足

- 当前用户在管理后台。
- 在{{<oem_name>}}已开启三级权限。
- 存储的共享范围为私有。
- 存储类型不为本地存储。
{{% /alert %}}

**单个块存储更改域**

1. 在左侧导航栏，选择 **_"存储/块存储/块存储"_** 菜单项，进入块存储页面。
2. 单击块存储右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"更改域"_** 菜单项，弹出更改域对话框。
2. 选择块存储所属的域，单击 **_"确定"_** 按钮。

**批量更改域**

1. 在块存储页面中勾选一个或多个块存储，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"更改域"_** 菜单项，弹出更改域对话框。
2. 选择块存储所属的域，单击 **_"确定"_** 按钮。


## 设置共享

该功能用于设置块存储的共享范围。

域资源的共享范围有三种：

- 不共享（私有）：即域资源只能本域的用户可以使用。
- 域共享-部分（多域共享）：即域资源可以共享到指定域（一个或多个），只有域资源所在域和共享域下的用户可以使用域资源。
- 域共享-全部（全局共享）：即域资源可以共享给全部域使用，即系统中所有用户都可以使用域资源。

{{% alert title="说明" %}}
设置共享的条件：需同时满足

- 当前用户在管理后台。
- 在{{<oem_name>}}已开启三级权限。
{{% /alert %}}

{{% alert title="注意" color="warning" %}}
本地存储的共享范围要始终要与宿主机的共享范围保持一致。
{{% /alert %}}

**单个块存储设置共享**

1. 在左侧导航栏，选择 **_"存储/块存储/块存储"_** 菜单项，进入块存储页面。
2. 单击块存储右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"设置共享"_** 菜单项，弹出设置共享对话框。
2. 配置以下参数：
   - 当共享范围选择为“不共享”时，即域资源的共享范围为私有，仅本域的用户可以使用。
   - 当共享范围选择为“域共享”时，需要选择共享的域。
       - 当域选择其中的一个或多个域时，即域资源的共享范围为域共享-部分，只有域资源所在域和共享域下的用户可以使用域资源。
       - 当域选择全部时，即域资源的共享范围为域共享-全部，系统中的所有用户都可以使用域资源。
3. 单击 **_"确定"_** 按钮，完成操作。

**批量设置共享**

1. 在块存储页面中选择一个或多个块存储，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"设置共享"_** 菜单项，弹出设置共享对话框。
2. 配置以下参数：
   - 当共享范围选择为“不共享”时，即域资源的共享范围为私有，仅本域的用户可以使用。
   - 当共享范围选择为“域共享”时，需要选择共享的域。
       - 当域选择其中的一个或多个域时，即域资源的共享范围为域共享-部分，只有域资源所在域和共享域下的用户可以使用域资源。
       - 当域选择全部时，即域资源的共享范围为域共享-全部，系统中的所有用户都可以使用域资源。
3. 单击 **_"确定"_** 按钮，完成操作。

## 删除

该功能用于删除块存储。当块存储未关联宿主机、且存储下没有硬盘文件和缓存文件时可删除。

{{% alert title="说明" %}}
- 本地存储不支持删除。
- 若块存储未关联宿主机、且存储下没有硬盘文件和缓存文件，仍删除不了存储，可能是硬盘文件未彻底删除存放在回收站中，请在回收站中清除硬盘。
{{% /alert %}}

1. 在左侧导航栏，选择 **_"存储/块存储/块存储"_** 菜单项，进入块存储页面。
2. 根据需要删除块存储的数量，选择删除方式。
    - 删除单个块存储：单击指定块存储右侧操作列 **_更多_** 按钮，选择下拉菜单 **_"删除"_** 菜单项，在弹出操作确认对话框中单击 **_"确定"_** 按钮。
    - 删除多个块存储：在存储列表中勾选一个或多个存储，单击列表上方 **_删除_** 按钮，在弹出操作确认对话框中单击 **_"确定"_** 按钮。
