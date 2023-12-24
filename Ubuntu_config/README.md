#Ubuntu16.04虚拟机下的一些配置和软件安装

##1、tool工具





## 2、python3环境和pip安装

###python3安装

[如何在 Ubuntu 18.04上安装 Python 3.8 - 云+社区 - 腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1626765)

[(85条消息) 如何将 Ubuntu 16 和 18 上的 python 升级到最新 3.8 版_haiiiiiyun的博客-CSDN博客_ubuntu升级python3.8](https://blog.csdn.net/haiiiiiyun/article/details/104771086?spm=1001.2101.3001.6650.2&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-2.pc_relevant_aa&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-2.pc_relevant_aa&utm_relevant_index=5)

安装python3.8后无法打开终端：[(85条消息) 安装python3.8后,Ubuntu无法打开终端gnome-terminal的解决方法整理版(importerror _gi)_LLY_A_的博客-CSDN博客_ubuntu 无法进入gnome](https://blog.csdn.net/LLY_A_/article/details/114385704?spm=1001.2101.3001.6650.10&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7ERate-10.pc_relevant_default&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7ERate-10.pc_relevant_default&utm_relevant_index=14)



### pip安装

[ubuntu18.04(python3.6)安装pip3报错：ImportError: cannot import name 'sysconfig' - 刘明野的博客 (liumingye.cn)](https://www.liumingye.cn/archives/250.html)



## 3、nodejs和npm安装

[ubuntu安装最新版node和npm - 简书 (jianshu.com)](https://www.jianshu.com/p/f2592d106aac)





## 4、yarn安装



## 5、nvim安装

很好的一个配置教程视频：[从零配置适合写C和C++的vim或neovim_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1dL411V75t?spm_id_from=333.999.0.0)

[Neovim+Coc.nvim配置 目前个人最舒服终端编辑环境(Python&C++) - zprhhs - 博客园 (cnblogs.com)](https://www.cnblogs.com/cniwoq/p/13272746.html)

1. 进入nvim的github主页下载deb包安装即可

2. 安装vim-plug

3. 在~/.config/nvim/init.vim中进行配置

   [使用 Vim 搭建 C/C++ 开发环境 - 不告诉你我是谁 - 博客园 (cnblogs.com)](https://www.cnblogs.com/kongj/p/14391151.html)

   ​

一些帮助网站：[记录neovim的点点滴滴 （入坑篇） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/76033635)

​			[使用 Vim 搭建 C/C++ 开发环境 - 码农教程 (manongjc.com)](http://www.manongjc.com/detail/23-wmnzlsrzdiffqhe.html)



### nvim中的插件安装

#### coc-nvim

[(85条消息) VIM——自动补全插件coc.nvim的安装与使用_盛气凌人666的博客-CSDN博客_coc.nvim](https://blog.csdn.net/bojin4564/article/details/105832148)

#### vimspector

[Vim 调试插件 Vimspector 基于 Dap (Debug Adapter Protocol) - 有翅膀的天狼 (josephpei.github.io)](http://josephpei.github.io/2020/02/01/vim-%E8%B0%83%E8%AF%95%E6%8F%92%E4%BB%B6-vimspector-%E5%9F%BA%E4%BA%8E-dap-debug-adapter-protocol/)

[vimspector C++调试 - 简书 (jianshu.com)](https://www.jianshu.com/p/ddcb374611e2)

[Vim 最强调试插件：vimspector - 不告诉你我是谁 - 博客园 (cnblogs.com)](https://www.cnblogs.com/kongj/p/12831690.html#%E4%BE%9D%E8%B5%96)

关键就是熟悉快捷键和配置.vimspector.json文件

个人是将配置文件上传到github，需要使用时克隆下来，并借助nvim中的配置文件的函数快速拷贝到当前目录





## 6、chrome安装

出现访问不了下载不了安装包时是/etc/hosts文件的问题，需要在里面添加chrome的访问地址



## 7、输入法安装



## 8、zsh

- 一个shell软件，和bash一样，在git管理的文件下可以显示分支情况



## 9、git安装和配置

出现生成秘钥方式不可用尝试使用Ed25519生成ssh秘钥[使用 Ed25519 算法生成你的 SSH 密钥 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/110413836)





### 10、unzip解压工具





## 11、ssh和sshd



## 12、编译工具g++，ccls、cmake，make

### 安装ccls

[Install ccls C/C++/ObjC Language Server on Ubuntu using the Snap Store | Snapcraft](https://snapcraft.io/install/ccls/ubuntu)



## 13、扩展系统盘工具

[(85条消息) **Ubuntu使用gparted扩展硬盘空间**_逗你玩^o^的博客-CSDN博客_ubuntu扩充磁盘空间gparted](https://blog.csdn.net/gaoxiangyyy/article/details/108977215)



## 14、网络配置

有关linux下的网络配置文件：

[(86条消息) linux--ubuntu网络配置_worthsen的博客-CSDN博客_ubuntu系统配置网络](https://blog.csdn.net/qq_38880380/article/details/99442543)

### 1、使用桥接

[(86条消息) 详细Ubuntu桥接模式网络配置过程_tiramisu_L的博客-CSDN博客_ubuntu桥接模式设置](https://blog.csdn.net/tiramisu_L/article/details/80557772)

注意事项：

[(86条消息) ubuntu16.04设置桥接模式，图文并茂，解决无法上网问题。_無荏知晓的博客-CSDN博客_ubuntu桥接模式无法上网](https://blog.csdn.net/Mr_jianfeng/article/details/81053849)

校园网只有一根网线，没法分配多余的静态IP，无法使用桥接方式

### 2、使用NAT

直接将网络适配器中的配置选择为NAT

并在VMware-》编辑-》虚拟网络编辑器-》更改设置-》选择NAT模式

### 3、代理配置

1. 打开网络设置，在代理一栏中添加

2. 查看主机IP和代理软件中代理的端口号

3. 分为http和socket，可以均配置。

   ![1651314922784](README.assets/1651314922784.png)

## FRP

服务端：运行于服务器的一个端口，只需修改配置文件（指定IP和端口号）并运行

客户端：只需配置IP（服务器的）和程序运行在服务器上的端口号和本地运行的端口号

### configuration

- server

```
[common]
bind_port = <server_port>
dashboard_port= <port_for_board>
dashboard_user=<user_name>
dashboard_pwd=<passwd>
#token用于验证，保证安全性
token=<what hell>
```

`./frps -c ./frps.ini`

- client

```
[common]
server_addr =<server_ip>
server_port =<server_port>
token =<what hell>
tls_enable =true # sometimes need

[RDP] # name is not important
type = tcp # maybe http
local_ip =127.0.0.1 #本地ip, 局域网ip
local_port =3389 # for windows
remote_port =<what you like>
```

`./frpc -c ./frpc.ini`

- usage

通过`<server_ip>:<what you like>`访问局域网

### issue

> 问题出现在：在云端服务器外还是有一个防火墙,需要通过网页操作打开