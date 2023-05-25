# WSL配置文件

## 子系统备份

- 定期导出更新备份

- 方便部署，本质就是docker

## windows terminal

- json配置文件

- 主要是快捷键

## zsh

- `.zshrc`

## nvim

- `~/.config/nvim/init.vim`

- `~/.config/nvim/coc-settings.json`

- nvim插件安装目录`~/.config/nvim/plugged`

- copilot安装

- 常用块编辑snippets，后续经常需要使用时学习

- 快编辑问题
  
  - v->进入visual模式
  
  - <C-q>进入visual block模式，可以进行多行编辑，选中多行后shift+i即可在选中的多行前面插入同样的内容

## ranger

- `~/.config/ranger/rc.conf`

- 在rc.conf中有能和fzf配合的使用的配置

## fzf

- 不要使用sudo安装

- 使用命令安装，同时保存按键绑定配置文件`/home/yong/.fzf/shell/key/bindings.zsh`

## 剪切板问题

- wsl->windows :正常复制粘贴

- vim->windows/windows->vim
  
  在vim配置文件中添加`set clipboard=unnamedplus`

## 网络问题

- 配置代理
  
  ```shell
  ## 获取主机 IP
  ## 主机 IP 保存在 /etc/resolv.conf 中
  # serverip为windows IP
  # hostip 为 WSL ip 二者虽然不同但本质是同个ip，两个均能连上网络
  export hostip=$(cat /etc/resolv.conf |grep -oP '(?<=nameserver\ ).*')
  export serverip=$(route.exe print | grep -a 0.0.0.0 | head -1 | awk '{print $4}')
  hostport=10811
  
  export https_proxy="http://${hostip}:${hostport}";
  export http_proxy="http://${hostip}:${hostport}";
  
  # export https_proxy="http://${serverip}:${hostport}";
  # export http_proxy="http://${serverip}:${hostport}";
  ```
