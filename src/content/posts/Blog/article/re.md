---
title: something
published: 2026-06-28
image: ../picture/太空.png
description: none
draft: false
---
# 软件
Lyricify
powertoys
flclash
project graph
# 代理调试指令
1. 代理端口切换:
```
git config --global http.proxy http://127.0.0.1:7890
git config --global https.proxy https://127.0.0:7890
```            
1. 查看已经配置代理:
```
git config --global --get http.proxy
git config --global --get https.proxy
```
1. 取消代理:
```
git config --global --unset http.proxy
git config --global --unset https.proxy
```