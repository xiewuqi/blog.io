---
layout: post
title: Mac 使用心得
date: 2017-10-23
categories: blog
tags: [编程,Mac]
description: 今天建立博客，放入博客。

---
> 某种工具的诞生必定带着某种创造精神

自己用的是15年的Mac por ，第一次用，刚开始从Windows转过来的时候很不习惯，不过我觉得每种系统都有它的优点和缺点，这是用 Mac 以来感觉做的不错的地方。多图，高手甚入。

##Mac官方文档
接触任何一项新东西的时候，就是查看他的官方文档。

[Mac官方文档](https://support.apple.com/zh-cn/explore/new-to-mac)
## 触控板
点击设置>触控板>查看手势用法
![](http://p85pnardv.bkt.clouddn.com/18-7-25/79307404.jpg)
![](http://p85pnardv.bkt.clouddn.com/18-7-25/93910874.jpg)



- 苹果在触控板上有很多特色，玩Mac的一定要好好看看。
- 手势的用法很酷吧？


## Mission Control
这有是 Mac 里一个非常好用的技能了，你可以同时建几个桌面，这个桌面用来播放娱乐软件，另一个
桌面用来当工作界面，还有一个用来监控电脑情况。
![](http://p85pnardv.bkt.clouddn.com/18-7-25/34674432.jpg)

- 用法很简单 触控板，三指往上拨就可以添加或者删除桌面了。



##      Spotlight     Alferd
- Spotlight 是Mac自带的搜索软件，搜索功能及其强大，这样让你不要鼠标的一个好技能。
`cmd + 空格   #快速呼出 Spolight `
![](http://p85pnardv.bkt.clouddn.com/18-7-25/10162179.jpg)

`option + 空格 #快速呼出 Alferd `


## homebrew  安装软件
官方网站：https://brew.sh
homebrew 是Mac 是一特殊的软件管理工具，不过需要操作终端，什么是终端呢？
` cmdmand + 空格 ` 直接搜索终端。

- 先下载 xcode ，这个在 app store 里面下载。
![](http://p85pnardv.bkt.clouddn.com/18-7-25/80453077.jpg)

- 安装 homebrew
在终端输入：
`ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

- 安装 homebrew cask
```
brew tap phinze/homebrew-cask
brew install brew-cask
```

#### 常用命令
```
安装软件：brew install 软件名
搜索软件：brew search 软件名
卸载软件：brew uninstall 软件名

显示已安装软件：brew list
查看那些已安装的程序需要更新： brew outdated
更新所有已安装软件：brew update && brew upgrade
```

#### 安装常用软件
```
brew cask install google-chrome  
brew cask install iterm2

brew cask install textmate
brew cask install evernote
rew cask install skitch             #ervernote配套的截图软件

brew cask install anki              #记忆软件

brew cask install alfred

```
- 如果你觉得一个一个的安装麻烦的话，可以这样。
```
brew cask install google-chrome && brew cask && install iterm2 && brew cask install textmate
 && brew cask install evernote && rew cask install skitch && brew cask install anki && brew cask install alfred
```
打包安装，这段时间你可以去喝杯咖啡，或者做点别的。

## iterm2 配置
安装iterm2：http://www.iterm2.com/
- iTerm2>Preference>keys>Hotkey:  可以设置自己喜欢的快捷键
- iTerm2>Preference>Profiles>Colors 配置颜色
- iTerm2>Preference>Profiles>Window>Miscellaneous>勾选Force 开头的那个


### 安装 zsh
`brew install zsh`  安装zsh
- 一般zsh自带的，不过一般不是最新版，这里重新安装一下。
`zsh --version` 查版本号
`echo $ZSH_VERSION` 查看当前使用版本
- 修改默认 shell
`sudo vi  /etc/shells` 
在 /etc/shells 里面增加一行 `/usr/local/bin/zsh ` 
退出 输出 `chsh -s /usr/local/bin/zsh`

### 安装 Oh My Zsh
Oh My Zsh 是一款自动配置zsh的软件
- 地址 http://ohmyz.sh/





## 参考
官网资料 https://support.apple.com/zh-cn/explore/new-to-mac
阳志平-mac效率手册 http://www.yangzhiping.com/tech/mac.html

## CHANGELOG
- 170617  创建
- 170618 增加homebrew内容
- 170712 增加 iterm2 配置
- 1712010 增加apple官网 
