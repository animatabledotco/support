---
description: >-
  This guide is no longer updated. It is for an old, outdated version of Limber
  (v1.7.5).
---

# Path to Bone

### &#x20;<img src="../.gitbook/assets/Button_0008_Path2Bone.png" alt="" data-size="original">&#x20;

Limber can instantly turn a path with three points into a bone with the same Stroke Width, Color, Tapering and so on.  **Path to Bone** is designed to be as simple to use as bones are to animate. For After Effects newcomers who just want to get animating simple characters as quickly as possible, or those upgrading from [Limber Lite](/broken/pages/6SzCJVuSn7K6Kk5RHtfz), Path to Bone is a great time-saver.&#x20;

You can either draw a path with After Effects' Pen tool, or import one from Illustrator and convert it to a shape layer.  The path needs to have exactly three points and there should be no other shapes in the layer. Tangents will be ignored. Limber will use the first Stroke property it finds in the layer for the new bone. It will place the start controller at the first point in the path and the end controller at the last, so **always draw your limb from the body outwards**.  After generating the bone, Limber turns off the visibility of the original path layer.

![](../.gitbook/assets/Path_to_Bone.gif)
