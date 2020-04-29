# autoremove-torrents-installation

## 目前支持的系统版本
`Ubuntu 16.04 / 18.04`、`Debian 8 / 9 / 10` 

## Install

```
bash <(wget -qO- https://github.com/DieNacht/autoremove-torrents-installation/raw/master/install -o /dev/null)
```

## Configure

```
bash <(wget -qO- https://github.com/DieNacht/autoremove-torrents-installation/raw/master/configure -o /dev/null) -u 用户名 -p 密码
```

## Set Alias

```
bash <(wget -qO- https://github.com/DieNacht/autoremove-torrents-installation/raw/master/alias -o /dev/null) -e 编辑器（仅支持nano/vim)
```

### Alias详细说明
命令`art`：和`autoremove-torrents`完全一致，仅为缩写

命令`art-execute`：为`autoremove-torrents -c $HOME/.config/autoremove-torrents/config.yml -l $HOME/.config/autoremove-torrents/logs`，其中$HOME为执行用户的HOME文件夹地址（ROOT用户：/root；非ROOT用户：/home/你的用户名）。执行时请保证$HOME/.config/autoremove-torrents/config.yml配置正确、$HOME/.config/autoremove-torrents/logs文件夹存在且执行用户有读写权限。

命令`art-configure`：为`nano/vim autoremove-torrents`，编辑器取决于你运行设置脚本的选择。如果系统没有安装相关编辑器，执行此命令会先执行编辑器安装（非ROOT用户执行安装，需确保系统装有sudoer且执行用户有sudo权限）。
