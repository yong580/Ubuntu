# wsl静态IP配置

在windows用户目录下的.wslconfig指定wsl使用的网络适配器，桥接到物理网卡，需要使用到Hyper-V管理器创建外部虚拟交换机，指定对应的网卡即可。

# 恢复使用主机的网络

只需将桥接相关的配置在.wslconfig中注释掉即可。



# VPN

只需在.bashrc或者.zshrc下获取主机IP（可以是子系统的NAT映射后的IP，也可以是windows主机IP，根据官网二者是一样的）并且根据VPN软件中的端口进行配置变量

```shell
export hostip=$(cat /etc/resolv.conf |grep -oP '(?<=nameserver\ ).*')
export serverip=$(route.exe print | grep -a 0.0.0.0 | head -1 | awk '{print $4}')
hostport=10811

export https_proxy="http://${hostip}:${hostport}";
export http_proxy="http://${hostip}:${hostport}";

# export https_proxy="http://${serverip}:${hostport}";
# export http_proxy="http://${serverip}:${hostport}";
```


