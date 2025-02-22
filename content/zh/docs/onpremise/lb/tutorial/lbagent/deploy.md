---
title: "部署节点"
date: 2021-12-22T14:54:38+08:00
weight: 20
description: >
    将负载均衡节点的配置文件下发到指定机器上
---

节点创建完成后需要将其部署在虚拟机、宿主机或外部机器上才能正常使用，部署节点的过程即将的配置文件下发到绑定的虚拟机上面。

{{% alert title="注意" color="warning" %}}
当转发节点上有监听任意IP的某个端口的服务配置时，会造成在使用该转发节点的LB实例上配置对应协议端口的监听无法正常使用。
```
# 在转发节点上查看监听任意IP的端口情况
$ netstat -nlp |grep 0.0.0.0:
tcp        0      0 0.0.0.0:22              0.0.0.0:*               LISTEN      7120/sshd
```
通过查询可以发现转发节点上的sshd服务正在监听任意IP的TCP 22端口，如用户需要在LB实例上配置TCP 22端口的监听，则需要将转发节点的sshd配置文件，将"/etc/ssh/sshd_config"配置文件的`#ListenAddress 0.0.0.0`改为`ListenAddress <转发节点IP>` 。
{{% /alert %}}

1. 在左侧导航栏，选择 **_"网络/负载均衡集群/负载均衡节点"_** 菜单项，进入负载均衡节点页面。
2. 单击节点右侧操作列 **_"部署"_** 按钮，弹出部署对话框。
2. 配置以下参数：
    - 指定系统用户：需要使用系统管理员用户部署节点。设置项目为“system”、选择已知密码的系统用户名并输入对应密码。如不存在已知系统用户密码，可通过climc命令创建系统用户lbagent用户，并使用lbagent用户及密码部署。
{{% alert title="说明" %}}
```bash
# 创建lbagent系统用户
$ climc user-create lbagent --password xxx --system-account 
# 将lbagent用户以管理员的角色加入到system项目
$ climc project-add-user system lbagent admin
```
{{% /alert %}}
    - 部署类型：选择转发实例节点，请尽量选取相互独立的虚拟机、宿主机或外部机器。
        - 当选择虚拟机时，要求虚拟机与负载均衡集群处于同一可用区，且虚拟机与控制节点网络连通。
        - 当选择宿主机时，要求宿主机与负载均衡集群处于同一可用区，且宿主机与控制节点网络连通。
        - 当选择外部机器时，要求ansible server（一般为控制节点）能够访问到目标机器。且目标机器上存在cloudroot用户，cloudroot用户支持sudo免密登录，管理员使用公钥可以免密登录cloudroot等。 
{{% alert title="说明" %}}
```bash
# 获取管理员公钥
$ climc sshkeypair-show --admin
``` 
{{% /alert %}}
    - Yum源地址：Yum源地址，[https://yunioniso.oss-cn-beijing.aliyuncs.com/iso/{version}/rpms](https://yunioniso.oss-cn-beijing.aliyuncs.com/iso/{version}/rpms)，且建议不勾选Yum源TLS校验。
     
3. 单击 **_"确定"_** 按钮，弹出部署对话框，查看节点的部署情况。
4. 若部署未执行完成，可再次单击 **_"部署"_** 按钮，在弹出的部署对话框中的单击”任务正在执行中框中“提示框的”详情“超链接，查看节点的部署情况。
5. 节点部署完成后，将显示节点的主备以及心跳信息等。