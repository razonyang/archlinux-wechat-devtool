# 微信开发者工具 for Arch Linux

**上游仓库已经停止更新了，该软件包也将不再维护。**

这个软件包已放在 [AUR](https://aur.archlinux.org/packages/wechat-devtool)，仅适用于 Arch Linux 及其衍生的发行版。
其他 Linux 平台，请移步原工具仓库：[微信开发者工具 for Linux](https://github.com/cytle/wechat_web_devtools)。

## 安装

> 安装的目录为 `/opt/wechat-devtool`。

```shell
$ git clone https://aur.archlinux.org/wechat-devtool.git
$ cd wechat-devtool
$ makepkg -si
```

也可以通过 AUR 工具安装，如 `aurman`：

```shell
$ aurman -S wechat-devtool
```

安装后，可以通过快捷方式启动，也可以命令行启动：

```
$ /opt/wechat-devtool/bin/wxdt
```

## 卸载

```shell
$ sudo pacman -R wechat-devtool
```

## 常见问题

### WeappVendor is not a directory

> cp: target '/home/user/.config/wechat_web_devtools/WeappVendor/' is not a directory

这是因为路径不存在，手动创建即可：

```shell
$ mkdir -p ~/.config/wechat_web_devtools/WeappVendor/
```
