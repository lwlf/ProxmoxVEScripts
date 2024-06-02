# RemovePVESubscriptionTip
一个移除 Proxmox VE 8 的订阅提示脚本，支持更新 proxmox-widget-toolkit 后自动移除订阅提示

# 使用说明

## 安装脚本

> 使用具有管理员权限的用户运行该命令

```shell
curl -OL https://github.com/lwlf/RemovePVESubscriptionTip/raw/main/removepvetip && mv removepvetip /usr/local/bin/removepvetip && chmod +x /usr/local/bin/removepvetip
```

## 脚本参数

### 开启屏蔽订阅提示

```shell
removepvetip --enable
```

### 关闭屏蔽订阅提示

```shell
removepvetip --disable
```

### 强制关闭（还原）屏蔽订阅提示，需要联网

```shell
removepvetip --force-disable
```

### 开启 hook，每次更新 proxmox-widget-toolkit 开启屏蔽订阅提示

```shell
removepvetip --hook
```

### 关闭 hook，每次更新 proxmox-widget-toolkit 不开启屏蔽订阅提示

```shell
removepvetip --unhook
```
