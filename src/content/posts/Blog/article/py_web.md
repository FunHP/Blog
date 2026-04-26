---
title: view py
published: 2026-04-22
description: python可视化web网页建立
image: ../picture/oo.png
tags: [py, visualize]
category: Learn
draft: false
---
> 项目实例：[PPO_Elevator](https://disk.dcpstudios.top/project/9)

<iframe width="100%" height="468" src="//player.bilibili.com/player.html?bvid=BV1RDQdBjEqo" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

# 结构
## 一、后端
1. [Flask](https://www.runoob.com/flask/flask-tutorial.html)
2. [Socket.IO](https://blog.csdn.net/gitblog_00825/article/details/150765996)
3. [RESTful_API](https://zhuanlan.zhihu.com/p/334809573)
## 二、前端
1. css
2. JavaScript

# 项目各文件类型功能分析

## Python 文件 (visualize_look.py)

### 核心功能
1. **LOOK 算法实现**
   - 实现完整的 LOOK 电梯调度算法
   - 智能方向控制和请求处理
   - 电梯状态管理

2. **后端服务**
   - Flask 应用服务器搭建
   - Socket.IO 实时通信
   - RESTful API 端点

3. **电梯环境模拟**
   - 电梯位置和状态管理
   - 乘客生成和处理
   - 电梯动作执行

4. **模拟控制**
   - 后台线程运行模拟
   - 速度控制和暂停/继续功能
   - 交通模式管理

5. **数据处理**
   - 状态数据收集和发送
   - 乘客请求处理
   - 统计数据计算

## JavaScript 文件 (index.html 中的 <script> 部分)

### 核心功能
1. **实时通信**
   - Socket.IO 客户端连接
   - 接收服务器状态更新
   - 发送控制命令

2. **3D 可视化**
   - 3D 大楼和电梯渲染
   - 电梯移动动画
   - 门开关效果

3. **用户交互**
   - 交通模式切换
   - FPS 控制
   - 播放/暂停控制

4. **数据可视化**
   - 等待时间趋势图表
   - 电梯动作历史记录
   - 实时统计数据显示

5. **UI 动态更新**
   - 电梯位置和状态更新
   - 乘客信息显示
   - 动画效果实现

## CSS 文件 (index.html 中的 <style> 部分)

### 核心功能
1. **3D 视觉效果**
   - CSS 3D 变换实现大楼透视
   - 电梯 3D 模型样式
   - 楼层和井道 3D 效果

2. **响应式布局**
   - 三栏布局设计
   - 自适应调整
   - 侧边栏和主内容区布局

3. **动画效果**
   - 电梯移动动画
   - 门开关过渡效果
   - 乘客上下电梯动画
   - 扫描线和尾迹效果

4. **主题设计**
   - 深色科技风格主题
   - 统一的色彩方案
   - 现代 UI 元素样式

5. **交互反馈**
   - 悬停效果
   - 按钮状态变化
   - 实时视觉反馈

## 技术协同关系

| 功能模块 | Python 后端 | JavaScript 前端 | CSS 样式 |
|---------|------------|----------------|----------|
| 电梯调度 | 实现 LOOK 算法逻辑 | 显示调度结果 | 美化显示效果 |
| 实时通信 | 发送状态数据 | 接收并处理数据 | - |
| 可视化效果 | - | 控制动画逻辑 | 提供视觉样式 |
| 用户控制 | 响应控制命令 | 发送控制请求 | 提供控制界面 |
| 数据统计 | 计算统计数据 | 展示统计结果 | 美化统计界面 |

## 技术特点总结

1. **Python 后端**：
   - 算法实现核心
   - 实时数据处理
   - 环境模拟引擎

2. **JavaScript 前端**：
   - 实时数据交互
   - 动态视觉效果
   - 用户交互处理

3. **CSS 样式**：
   - 3D 视觉呈现
   - 现代 UI 设计
   - 流畅动画效果

这种前后端分离的架构设计，使得系统既具备强大的算法处理能力，又拥有直观美观的用户界面，为电梯调度算法的研究和教学提供了理想的可视化工具。