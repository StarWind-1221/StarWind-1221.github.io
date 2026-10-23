---
title: 卡尔曼滤波公式推导
math: true
categories: 知识学习
---

<!--more-->

# VMware 安装 Debian 13 记录

1. 将当前用户添加进 sudoers，方便进行 sudo
    ```bash
    su -
    usermod -aG sudo username
    reboot
    ```

2. 更换软件源，[Debian 清华源]([https://mirrors.tuna.tsinghua.edu.cn/help/debian/](https://mirrors.tuna.tsinghua.edu.cn/help/debian/))，选择 DEB822 格式（记得清空旧格式文件内容）
  ```bash
  sudo apt update && sudo apt upgrade
  ```

3. 生成 ssh keys，并添加到 github 账户，下载 dotfiles 仓库

    ```bash
    ssh ssh-keygen -t ed25519 -C "your_email@example.com"
    ```

4. 安装 vim 和 curl
    ```bash
    sudo apt install vim curl -y
    ```

5. 配置代理

6. 安装 vmtools
    ```bash
    sudo apt install open-vm-tools open-vm-tools-desktop -y
    vmware-toolbox-cmd -v
    ```

## 不需要进行的配置

1. 终端，直接利用 ssh 进行远程访问
2. 系统时钟设置