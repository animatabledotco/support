---
description: >-
  This guide is for an outdated version of Penpal (1.5.0) - please visit
  https://penpal.docs.animatable.co for the current user guide.
---

# Tangents tab

![](<.gitbook/assets/tangentsstab (1).png>)

{% hint style="warning" %}
When dealing with tangents, remember that even a ‘zero’ tangent, is treated by Penpal as a selectable element. If you drag a marquee selection over a point with zero tangents, you’ll be selecting both tangents.
{% endhint %}

#### <img src=".gitbook/assets/points - up.svg" alt="" data-size="line"> Move up,<img src=".gitbook/assets/points - down.svg" alt="" data-size="line"> Move down, <img src=".gitbook/assets/points - left.svg" alt="" data-size="line"> Move left, <img src=".gitbook/assets/points - right.svg" alt="" data-size="line"> Move right

These buttons move selected tangents by 1px, or 10px if you hold `Shift`

#### <img src=".gitbook/assets/tangents - copy.svg" alt="" data-size="line"> Copy

Copies the selected tangents. You can copy _one_ or _both_ tangents _of a pair_. You cannot copy tangents from different points.

#### <img src=".gitbook/assets/tangents - paste.svg" alt="" data-size="line"> Paste

Pastes the copied tangents to the selected tangents. You can paste to multiple tangents simultaneously.

If you copy **and** paste both In **and** Out tangents, they will paste in-to-in and out-to-out. If you copied **only one** tangent of a pair, and you paste to **only one** tangent, you will paste the tangent you copied, end of. Also see [Advanced tangent pasting](advanced-tangent-pasting.md) on the next page.

#### <img src=".gitbook/assets/tangents - zero.svg" alt="" data-size="line"> Zero

Zero’s out the selected tangents. You can also zero tangents by pressing the `Backspace` (delete) key on your keyboard, when in the Tangents tab.

#### <img src=".gitbook/assets/tangents - flatV.svg" alt="" data-size="line"> Flatten to vertical axis, <img src=".gitbook/assets/tangents - flatH.svg" alt="" data-size="line"> Flatten to horizontal axis

Rotates selected tangents around their parent point, to the nearest spot on it's vertical or horizontal axis. These axes are in the current [Space](spaces.md).

#### <img src=".gitbook/assets/tangents - flipV.svg" alt="" data-size="line"> Flip around vertical axis, <img src=".gitbook/assets/tangents - flipH.svg" alt="" data-size="line"> Flip around horizontal axis

Rotates the selected tangents so that they flip over the vertical or horizontal axis of their parent point. These axes are in the current [Space](spaces.md)

#### <img src=".gitbook/assets/tangents - swap.svg" alt="" data-size="line"> Swap

This button swaps a pair of tangents with one another.

#### <img src=".gitbook/assets/tangents - matchLength.svg" alt="" data-size="line"> Match length

Makes the selected tangents the same length as their opposite. If you only selected _one_ tangent of a pair, it will become the same length as the other. If you select _both_ tangents of a pair, both will be altered to their average length.

#### <img src=".gitbook/assets/tangents - opposeAngle.svg" alt="" data-size="line"> Match angle

Rotates a selected tangent so that it is exactly 180º to it's opposite, and set the point to _smooth_ (the tangent handles are linked to one another to maintain a straight line as you drag them around). If you select both tangents of a pair, their angles will be averaged and then each one set to +90º and -90º from this average.

#### &#x20;<img src=".gitbook/assets/tangents - facePoint.svg" alt="" data-size="line"> Align to point

Rotates a selected tangent so that it aligns directly toward it's neighbouring point. Eg. an In tangent will face toward the previous point and an Out tangent will face toward the next point.

#### <img src=".gitbook/assets/tangents - rotate.svg" alt="" data-size="line"> Rotate

This button will rotate tangents by a value, specified in degrees, around their parent point. Holding the `Alt` key will make it rotate in the opposite direction. Hover over the button and click the gear icon to [Set Rotation value](tangents-tab.md#set-rotation-value).

#### <img src=".gitbook/assets/tangents - setRotate.svg" alt="" data-size="line"> Set Rotation value

This button sets a value, in degrees, which the [Rotate](tangents-tab.md#rotate) button applies.
