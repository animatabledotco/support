---
description: >-
  This guide is for an outdated version of Penpal (1.5.0) - please visit
  https://penpal.docs.animatable.co for the current user guide.
---

# Paths tab

![](.gitbook/assets/pathstab.png)

The functions in the Paths tab tend to affect the shape as a whole, rather than it’s individual points.

{% hint style="warning" %}
When we refer to a path’s **bounding box** we mean the rectangle formed by it’s outermost visible parts.
{% endhint %}

#### <img src=".gitbook/assets/paths - center.svg" alt="" data-size="line"> Center

Center the path in the composition, layer or shape group, depending on which Space you have active.&#x20;

#### <img src=".gitbook/assets/paths - centerV.svg" alt="" data-size="line"> Center vertically,  <img src=".gitbook/assets/paths - centerH.svg" alt="" data-size="line"> Center horizontally

Vertically or horizontally center the path, as above.

#### <img src=".gitbook/assets/paths - flipV.svg" alt="" data-size="line"> Flip vertically, <img src=".gitbook/assets/paths - flipH.svg" alt="" data-size="line"> Flip horizontally

Flip the path top-to-bottom or left-to-right, around its  center.

#### <img src=".gitbook/assets/paths - flipT.svg" alt="" data-size="line"> Flip up, <img src=".gitbook/assets/paths - flipB.svg" alt="" data-size="line"> Flip down,  <img src=".gitbook/assets/paths - flipR.svg" alt="" data-size="line"> Flip right,  <img src=".gitbook/assets/paths - flipL.svg" alt="" data-size="line"> Flip left

Flip the path around the top, bottom, right or left edge of its  bounding box.

#### <img src=".gitbook/assets/paths - reverse.svg" alt="" data-size="line"> Reverse

Reverse the order of the points in the selected path. It’s first vertex will remain the same, unless you apply it to an open path, in which case the first vertex will be moved to the opposite end.

#### <img src=".gitbook/assets/paths - open.svg" alt="" data-size="line"> Toggle open

Toggle selected paths from open to closed, or vice versa. If you have multiple paths selected, you can hold `Alt` to make them all open, or `Cmd/Ctrl` to make them all closed.

#### <img src=".gitbook/assets/paths - simplify.svg" alt="" data-size="line"> Simplify

This function removes points from the selected paths whilst attempting to preserve their basic shape. When you hover over the button, it brings up a slider below. Drag the slider to the right to reduce the number of points and Penpal will preview how your paths will be simplified. To apply it, click the blue checkmark icon. If you move your cursor away from the slider container, the process is aborted.

#### <img src=".gitbook/assets/paths - join.svg" alt="" data-size="line"> Join

This button will join two or more open paths into one. Paths are joined in the order they were selected in the canvas, and from each one's last point to the next one's first point (following their direction). A new, joined path is created, and the original paths are turned off in the timeline. If your paths seem to join at the wrong ends you probably need to [reverse](path-tab.md#reverse) one or more of them before you join them.

{% hint style="warning" %}
The Join function currently does not support masks, it only works with shape paths.
{% endhint %}

