---
description: >-
  This guide is for an outdated version of Penpal (1.5.0) - please visit
  https://penpal.docs.animatable.co for the current user guide.
---

# Advanced tangent pasting

Following on from [Paste Tangents](tangents-tab.md#paste), here are the more advanced methods available for pasting tangents in Penpal.

**If you copied&#x20;**_**both**_**&#x20;tangents from a pair, and paste to&#x20;**_**only one**_**&#x20;tangent of a pair**, which tangent is pasted will depend on which tangent you have _selected_: if you have the In tangent selected, Penpal will paste the copied In tangent. If you have the Out tangent selected, Penpal will paste the copied Out tangent.

**If you copied&#x20;**_**only one**_**&#x20;tangent from a pair, and paste to&#x20;**_**both**_**&#x20;tangents of a pair**, which tangent is altered depends on which tangent you _copied_. If you copied the In tangent, the selected In tangent will be pasted to. If you copied the Out tangent, the selected Out tangent will be pasted to.

#### <img src=".gitbook/assets/tangents - pasteLength.svg" alt="" data-size="line"> Paste Length and <img src=".gitbook/assets/tangents - pasteAngle.svg" alt="" data-size="line"> Paste Angle

If you hover over the Paste button, there are additional buttons to paste only the length or only the angle. If you paste length, the selected tangents will retain their existing angles. If you paste angle, the selected tangents will retain their existing length.

All three Paste buttons have a unique, super-local method of pasting that attempts to paste tangents relative to the angle of the neighbouring points. This mode is activated when you hold `Cmd/Ctrl` on clicking the Paste buttons. For example, if you make a many-sided polygon and then adjust the tangents of one point, copy them, and then paste to the other tangents holding `Cmd/Ctrl`, each pair of tangents will rotate the tangents to match the outer surface of the polygon.

Copying and pasting tangents is not affected by changes to the Space. It's always performed within Local space, regardless of which Space you have active.
