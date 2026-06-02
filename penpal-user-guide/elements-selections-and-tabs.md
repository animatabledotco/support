---
description: >-
  This guide is for an outdated version of Penpal (1.5.0) - please visit
  https://penpal.docs.animatable.co for the current user guide.
---

# Tabs and selections

## Tabs

There are three tabs at the top of the panel, denoted by symbols: <img src=".gitbook/assets/tabs - paths.svg" alt="" data-size="line">Paths, <img src=".gitbook/assets/tabs - points.svg" alt="" data-size="line">Points and <img src=".gitbook/assets/tabs - tangents.svg" alt="" data-size="line">Tangents. Clicking on these tabs displays different groups of buttons, and highlights the relevant elements in the canvas. [Path functions](path-tab.md) affect the path as a whole - it will maintain it’s proportions and essential shape. [Point functions](points-tab.md) affect points and [Tangent functions](tangents-tab.md) affect tangents.

## Selections

You can select elements by dragging a marquee over them, or by clicking on them one-by-one while holding `Shift` or `Cmd/Ctrl`.

[Paths](path-tab.md) can only be selected by dragging.

**Selecting elements in the canvas is not dependent on tab - you can still select points while you're in the tangents tab, and so on.**

Unselected points and tangents are displayed with an outlined icon. When they are selected, it becomes filled. Selected paths are slightly brighter in the points and tangents tabs, and blue when in the paths tab.

{% hint style="warning" %}
Unlike Adobe software generally, selecting a point does **not** automtically select it’s tangents. In Penpal, they are treated as separate things. To select both tangents of a pair, you need to drag the marquee over both of them, or Shift-click on them one-by-one.
{% endhint %}
