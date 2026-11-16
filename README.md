# Iris小手机

Iris小手机正式版。前端可通过 GitHub Pages 部署，后端可在小手机内一键搭建。

[打开 Iris小手机](https://weishengrongqing-commits.github.io/Iris/) · [Fork 仓库](https://github.com/weishengrongqing-commits/Iris/fork)

## 部署自己的小手机

1. 点击仓库右上角 **Fork**，复制到自己的 GitHub 账号。
2. 在自己的仓库打开 **Settings → Pages**。
3. Source 选择 **Deploy from a branch**，分支选择 **main**，目录选择 **/ (root)**，点击 **Save**。
4. 等待 Pages 发布完成；页面会显示网站链接，点击 **Visit site** 即可打开自己的小手机。通常地址为 `https://你的用户名.github.io/你的仓库名/`。

## 一键部署后端

打开自己的小手机，进入 **全局设置 → 部署**：

- **使用公共服务**：选择音乐、后台通知，点击「连接公共服务」，无需登录 Cloudflare。
- **自己搭建**：点击「登录并授权」，选择 Cloudflare 账户、服务和后端地址，再点击「搭建并连接」。全程在小手机内完成，无需运行命令。

自建后端部署在你自己的 Cloudflare 账户，使用自己的额度。可使用自动分配的 `workers.dev` 地址，也可绑定已添加到该账户的域名。搭建完成后，可在「查看服务地址」中确认地址。

聊天模型的 URL、Key 和模型仍在全局设置中自行配置。后台通知需设备和浏览器支持系统推送。

## 文件说明

| 位置 | 用途 |
| --- | --- |
| `index.html`、`style.css` | 网页入口和界面样式 |
| `scripts/` | 功能页面和前端逻辑 |
| `config/` | 版本、安装清单及服务地址 |
| `cloudflare/` | 音乐、通知和自助部署服务源码 |
| `assets/` | 图片、字体、地图和素材许可 |
| `docs/` | 使用及维护说明 |
| `tests/`、`tools/` | 自动检查和维护工具 |

详细步骤见 [部署说明](docs/部署说明.md)。
