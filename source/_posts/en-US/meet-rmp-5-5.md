---
title: Meet Rail Map Painter 5.5!
date: 2026-06-16 00:00:00
lang: en-US
tags:
  - RMP
  - Update
---

Rail Map Painter 5.5 is here! This update focuses on freer line drawing, more flexible style composition, favorite tools, reusable specific attributes, and a new set of line badges and regional style additions, making complex map editing smoother.

---

## 🧭 Arbitrary Angle Segments

The new "Arbitrary angle path" lets you set separate start and end angles, then adjust start/end offsets and rounded corners. It is useful for drawing bends that are not limited to 45°, 90°, or other fixed directions, so routes can follow the shape of the reference map more closely.

<video src="/rmt-blog/images/rmp-5-5/ray-guided-line.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🧱 Generic Line Style

The new "Generic style" lets you build one line style from multiple stacked layers. Each layer can have its own color, width, opacity, line cap, dash length, and gap length. Layers can also be copied, reordered, or removed, making it easier to create special routes, legend lines, or temporary visual schemes.

<video src="/rmt-blog/images/rmp-5-5/generic-line-style.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## ⭐ Favorite Tools

The left tools panel now supports favorites. Frequently used line styles, stations, and miscellaneous nodes can be favorited, then filtered with "Show only favorites" to reduce time spent searching long lists.

<video src="/rmt-blog/images/rmp-5-5/favorite-tools.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🎛️ Line Style Preview Icons

The line style list now shows preview icons rendered from the actual styles. Before choosing a style, you can already see its visual appearance, which is especially helpful for style-rich systems such as London, JR East, MTR, and intercity railways.

![Line style preview icons](/rmt-blog/images/rmp-5-5/line-style-icons.png)

---

## 📋 Copy and Paste Specific Attributes

The context menu now includes "Copy Specific Attributes" and "Paste Specific Attributes". Between stations of the same type, miscellaneous nodes of the same type, or lines using the same style, you can reuse only the specific attributes without changing names, positions, or other basic information.

<video src="/rmt-blog/images/rmp-5-5/copy-paste-specific-attrs.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🔗 Select Connected Lines with the Same Style

Double-click a line segment to select all connected segments with the same style. When you need to adjust the style, layer order, or attributes of one continuous route section, you no longer need to multi-select segment by segment.

<video src="/rmt-blog/images/rmp-5-5/select-connected-lines.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🚅 Shinkansen Style

The new JR East Shinkansen style draws routes with directional arrow details. It supports common path types and can be used together with terminal decorations.

![Shinkansen style](/rmt-blog/images/rmp-5-5/shinkansen.png)

---

## 🚉 JR East Terminal Decorations

JR East single color style and JR East single color filled with crosshatch pattern style now support terminal decoration settings. You can choose displays such as "Terminal" or "Other line section", and specify whether the decoration appears at the start or end of the segment.

![JR East terminal decoration 1](/rmt-blog/images/rmp-5-5/jr-east-terminal-decoration-1.png)

![JR East terminal decoration 2](/rmt-blog/images/rmp-5-5/jr-east-terminal-decoration-2.png)

---

## 🚇 London Tube Line Badge

The new London Tube line badge node supports regular line badges and walking badges. Badges can include a line name, walking target, and distance, and multiple badge items can be stacked for London-style notes and interchange information.

![London Tube line badge](/rmt-blog/images/rmp-5-5/london-tube-line-badge.png)

---

## 🏙️ Wuhan Rail Transit Badges

The Wuhan Rail Transit line badge node has been added, and Wuhan interchange stations now support icons for three or more lines plus editable transfer information. Wuhan-style maps can now present line numbers and interchange symbols more completely.

![Wuhan Rail Transit badges](/rmt-blog/images/rmp-5-5/wuhan-rt-badges.png)

---

## 🚏 Shenzhen Facility Icons

New Shenzhen facility icons are available for railway stations, intercity railway, ferries, trams, and airports, making it easier to show more transport connections on Shenzhen-related maps.

![Shenzhen facility icons](/rmt-blog/images/rmp-5-5/shenzhen-facilities.png)

---

## ✨ Other Improvements

- The line path data structure and calculation logic have been refactored, making offsets, strokes, outlines, and rounded corners more stable.
- Empty station names can now be used when creating stations, which helps when filling names later or drafting maps without station names.
- Station names can now be dragged directly to a custom position.
- Node coordinate inputs are more robust, and invalid values are no longer written directly into the project.
- Shanghai 2024 facility icons have been updated.
- Guangdong Intercity Railway style now has a gray color option.
- Guangzhou Metro line badges now support the APM-style line box.
- Beijing Subway interchange icons have been updated and repositioned.
- Changsha Metro interchange stations now have a color-flip option, with station name positioning fixes.
- Canvas dragging, zooming, node dragging, grid lines, and selected-element highlighting have been improved, with smoother touchpad and mobile interactions.
- Image and SVG export cleanup and Safari compatibility have been improved, with fixes for empty canvas export, attribution options, and special SVG path export issues.
