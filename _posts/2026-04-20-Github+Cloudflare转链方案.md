---
title: Github+Cloudflare转链方案
date: 2026-04-20 16:59:13 +08:00
author: <gaoshouq>
categories:
  - 个人站
tags:
  - 博客
---
# 所需要准备的内容
- 一个 GitHub 账号（已有）
- 一个**自己的域名**（必须，几块钱一年）
- Cloudflare 账号（免费注册）
# 流程
- **博客正常部署到 GitHub Pages**
    用 `xxx.github.io` 域名能正常访问。
- **买一个便宜域名**
    比如 Namesilo、Namecheap 都行，一年几块钱。
- **把域名 DNS 改成 Cloudflare**
    Cloudflare 会给你两个 DNS 服务器，去域名商后台替换。
- **在 Cloudflare 里绑定你的 GitHub Pages**
    - 添加你的域名
    - 设置 DNS 记录指向 GitHub Pages
    - 开启**代理模式（橙色云）**
- **开启强制 HTTPS、缓存策略**
    博客静态文件（HTML/CSS/JS/ 图片）会被 Cloudflare 全球节点缓存。
·
