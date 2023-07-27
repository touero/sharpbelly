<h1 align="center">为wsl设置本机代理</h1>



<p align="center">
<img src="https://img.shields.io/badge/python_-%3E%3D3.8-green" alt=""> <img src="https://img.shields.io/badge/license_-MIT-green" alt=""> <img src="https://img.shields.io/badge/shell-blue" alt=""> <img src="https://img.shields.io/badge/zsh-blue" alt="">  <img src="https://img.shields.io/badge/bash-blue" alt=""> 
</p>

## 仓库介绍

&emsp;&emsp;实际开发中需要在wsl中使用代理, 这个仓库为解决wsl快捷设置代理, 快捷取消设置代理提供支持.


## 安装

这个项目使用[WSL](https://learn.microsoft.com/en-us/windows/wsl/install) [Git](https://git-scm.com/) 请确保你本地安装了它们, 同时确保你的代理客户端运行局域网代理, 即 Allow LAN。

```shell
$ git clone https://github.com/weiensong/wslProxy.git

# !!! 进入拉取目录, 设置其中端口port !!!

# 移动至/data/tools
$ sudo mv proxy.sh /data/tools/proxy.sh

# !!! 确认使用的shell,当前使用zsh,设置到alias !!!

$ nvim ~/.zshrc
# 增加以下内容:
alias proxy='source /data/tools/proxy'
```


## 运行
```sh
# 开启代理
$ proxy set

# 关闭代理
$ proxy unset

# 输出代理信息
$ proxy test

# 测试代理
# curl google.com
```

## 相关仓库

- [zsh](https://github.com/zsh-users/zsh) — Mirror of the Z shell source code repository
- [clash](https://github.com/Dreamacro/clash) — A rule-based tunnel in Go
- [v2rayN](https://github.com/2dust/v2rayN) — A GUI client for Windows, support Xray core and v2fly core and others
- [ohmyzsh](https://github.com/ohmyzsh/ohmyzsh) — delightful community-driven (with 2,100+ contributors) framework for managing your zsh configuration. Includes 300+ optional plugins (rails, git, macOS, hub, docker, homebrew, node, php, python, etc), 140+ themes to spice up your morning, and an auto-update tool so that makes it easy to keep up with the latest updates from the community.



## 相关链接

- [wsl](https://learn.microsoft.com/en-us/windows/wsl/install)



## 维护者

[@weiensong](https://github.com/weiensong)



## 如何贡献

非常欢迎你的加入！[提一个 Issue](https://github.com/weiensong/wslProxy/issues) 或者提交一个 Pull Request。


标准遵循 shell 行为规范。

### 贡献者

感谢参与项目的所有人



## 使用许可

[MIT](LICENSE) © weiensong

