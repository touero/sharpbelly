<h1 align="center">Set up a native proxy for wsl</h1>



<p align="center">
<img src="https://img.shields.io/badge/license_-MIT-green" alt=""> <img src="https://img.shields.io/badge/shell-blue" alt=""> <img src="https://img.shields.io/badge/zsh-blue" alt="">  <img src="https://img.shields.io/badge/bash-blue" alt=""> 
</p>

## Repository Introduction

In actual development, it is necessary to use proxies in wsl. This repository provides support for quickly setting proxies and quickly canceling proxy settings in wsl.


## Install

This project uses [WSL](https://learn.microsoft.com/en-us/windows/wsl/install) [Git](https://git-scm.com/) Go check them out if you don't have them locally installed, At the same time, ensure that your proxy client allows LAN proxies, that is, Allow LAN.

```shell
$ git clone https://github.com/weiensong/wslProxy.git

# ❗❗❗ Enter the pull directory and set the port in it ❗❗❗

# move to /data/tools
$ sudo mv proxy.sh /data/tools/proxy.sh

# ❗❗❗ Confirm the shell used, currently using zsh, set to alias ❗❗❗

$ nvim ~/.zshrc
# Add the following content:
alias proxy='source /data/tools/proxy.sh'

$ source ~/.zshrc
```


## Usage
```sh
# Enable Proxy
$ proxy set

# Able Proxy
$ proxy unset

# Output proxy information
$ proxy test

# Test proxy
$ curl google.com
```

## Related Repository

- [zsh](https://github.com/zsh-users/zsh) — Mirror of the Z shell source code repository
- [clash](https://github.com/Dreamacro/clash) — A rule-based tunnel in Go
- [v2rayN](https://github.com/2dust/v2rayN) — A GUI client for Windows, support Xray core and v2fly core and others
- [ohmyzsh](https://github.com/ohmyzsh/ohmyzsh) — delightful community-driven (with 2,100+ contributors) framework for managing your zsh configuration. Includes 300+ optional plugins (rails, git, macOS, hub, docker, homebrew, node, php, python, etc), 140+ themes to spice up your morning, and an auto-update tool so that makes it easy to keep up with the latest updates from the community.



## Related Efforts

- [wsl](https://learn.microsoft.com/en-us/windows/wsl/install)



## Maintainers

[@weiensong](https://github.com/weiensong)


## Contributing

Feel free to dive in! [Open an issue](https://github.com/weiensong/scrapySelenium/issues)[Open an issue](https://github.com/weiensong/wslProxy/issues) or submit PRs.

Standard Python follows the Shell Code of Conduct.

### Contributors

This project exists thanks to all the people who contribute.


## License

[MIT](LICENSE) © weiensong

