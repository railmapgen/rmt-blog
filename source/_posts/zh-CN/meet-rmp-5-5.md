---
title: 遇见地铁线路图绘制器 5.5！
date: 2026-06-16 00:00:00
lang: zh-CN
tags:
  - RMP
  - 更新
---

地铁线路图绘制器 5.5 来了！本次更新围绕更自由的线路绘制、更灵活的样式组合、常用工具管理、属性复用，以及一批线路标识和地区样式补充展开，让复杂线路图的制作过程更顺手。

---

## 🧭 任意角度线段

新增“任意角度线段”，可以分别设置起点和终点的角度，并调整起终点偏移与圆角因子。它适合绘制不局限于 45°、90°或固定方向的折线，让线路走向更贴近真实图面需求。

<video src="/rmt-blog/images/rmp-5-5/ray-guided-line.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🧱 通用线段样式

新增“通用样式”，支持把多层线条叠加成一个线路样式。每一层都可以设置颜色、宽度、透明度、线帽、虚线长度和间隔，也可以复制、排序或删除，用来制作特殊线路、图例线或临时视觉方案都更方便。

<video src="/rmt-blog/images/rmp-5-5/generic-line-style.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## ⭐ 收藏常用工具

左侧工具面板新增收藏功能。常用的线路样式、车站和杂项节点可以加入收藏，并通过“仅显示收藏”快速过滤，减少在长列表中反复寻找工具的时间。

<video src="/rmt-blog/images/rmp-5-5/favorite-tools.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🎛️ 线路样式预览图标

线路样式列表现在会显示实际样式预览图标。选择样式前就能看到大致视觉效果，尤其在伦敦、JR East、MTR、城际铁路等样式较多的场景下更直观。

![线路样式预览图标](/rmt-blog/images/rmp-5-5/line-style-icons.png)

---

## 📋 复制与粘贴独特属性

右键菜单新增“复制独特属性”和“粘贴独特属性”。同类型车站、同类型杂项节点或同样式线段之间，可以只复用独特属性，而不影响名称、位置或其他基础信息。

<video src="/rmt-blog/images/rmp-5-5/copy-paste-specific-attrs.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🔗 一键选中相连同样式线段

双击线段即可选中所有相连且样式相同的线段。需要批量调整同一段线路的样式、层级或属性时，不再需要逐段多选。

<video src="/rmt-blog/images/rmp-5-5/select-connected-lines.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🚅 新干线样式

新增 JR East 新干线线路样式，可绘制带方向箭头质感的线路。它支持常见线段类型，并可配合终端装饰一起使用。

![新干线样式占位图](/rmt-blog/images/rmp-5-5/shinkansen.png)

---

## 🚉 JR East 终端装饰

JR East 单色样式和网状图案样式新增终端装饰设置，可选择“终点”或“其他线区”等显示方式，并指定装饰显示在线段起点或终点。

![JR East 终端装饰占位图1](/rmt-blog/images/rmp-5-5/jr-east-terminal-decoration-1.png)

![JR East 终端装饰占位图2](/rmt-blog/images/rmp-5-5/jr-east-terminal-decoration-2.png)

---

## 🚇 伦敦地铁线路标牌

新增伦敦地铁线路标牌节点，支持普通线路标牌与步行标牌。标牌可填写线路名、步行目标和距离，也可以堆叠多个项目，适合制作更接近伦敦图面风格的说明与换乘信息。

![伦敦地铁线路标牌](/rmt-blog/images/rmp-5-5/london-tube-line-badge.png)

---

## 🏙️ 武汉轨道交通标识

新增武汉轨道交通线路标识节点，同时武汉换乘站支持 3 线及以上换乘图标和换乘信息编辑。制作武汉风格线路图时，线路编号和换乘图形可以更完整地呈现。

![武汉轨道交通标识占位图](/rmt-blog/images/rmp-5-5/wuhan-rt-badges.png)

---

## 🚏 深圳设施图标

新增深圳火车站、城际铁路、轮渡、有轨电车和机场设施图标，便于在深圳相关线路图中标注更多交通接驳信息。

![深圳设施图标占位图](/rmt-blog/images/rmp-5-5/shenzhen-facilities.png)

---

## ✨ 其他改进

- 重构了线段路径的数据结构与计算方式，现在能更稳定地参与偏移、描边、轮廓和圆角处理。
- 创建车站时可直接使用空白站名，适合后续统一补名或制作无站名草图。
- 车站名称支持直接拖动到自定义位置。
- 节点坐标输入更稳健，非法值不会直接写入项目。
- 更新上海 2024 设施图标。
- 广东城际铁路样式新增灰色选项。
- 广州地铁线路标识支持 APM 样式线框。
- 北京地铁换乘图标更新并修正位置。
- 长沙换乘站新增颜色翻转选项，并修正站名位置。
- 优化画布拖拽、缩放、节点拖动、网格线与选中高亮等体验，触控板和移动端操作也更顺手。
- 改进图片和 SVG 导出清理与 Safari 兼容性，并修复空画布、署名选项和特殊 SVG path 的导出问题。
