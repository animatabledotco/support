---
description: >-
  This guide is no longer updated. It is for an old, outdated version of Limber
  (v1.7.5).
---

# Managing controllers

### Hiding and showing Controllers

### <img src="../.gitbook/assets/Button_0004_Hide.png" alt="" data-size="original">&#x20;

You can hide controllers by clicking **Hide/Show** when you have one or more Limber layers selected. Limber will then hide all the controllers from that set.  If you have no Limber layers selected, it'll hide all the controllers in your comp.  **Alt**-clicking the Hide/Show button will show controllers again in the same manner.  Hiding and showing controllers turns their opacity to 0 or 100 rather than affecting the visibility switch for the layers, so that you can still see and edit the motion path when you select a hidden controller.

{% hint style="info" %}
You can use the layer visibility (eyeball) switches for a second level of control over hiding.  For example: to permanently turn off the visibility of just your start controllers, since they are often not keyframed at all.
{% endhint %}

Start and end controllers gradually shift color when they are moved close to the limb's fully stretched out length. When they reach the same distance as the limb's total length (and the limb becomes dead straight) they change abruptly to red. This makes it easier to spot pops when you are animating. You can disable these color changes by **shift**-clicking the **Hide/Show** button.  Shift-clicking again will turn the color dynamics back on. You can disable color dynamics on all newly generated limbs in the [settings panel](../getting-started/settings-panel.md).

### Changing Controller Size

### <img src="../.gitbook/assets/Button_0009_Size.png" alt="" data-size="original">&#x20;

You can make controllers larger or smaller by clicking (or **alt**-clicking) the **+/- Size** button. This will re-size all the controllers from the selected limb set.

### Controller Rotation

The automatic rotation of controllers, which you determine using the Rotate Start and Rotate End properties in the Limber effect, takes effect through an expression on their Rotation properties. This allows for you to parent your own layers to Limber's controllers, and have those layers stay aligned to the angles of the limb.

By default, these rotation properties cannot be altered by the user. If you want to animate the rotation of your own hand and feet layers, you'd need to do it by keyframing the rotation property of those layers themselves, and you may need to adjust their anchor points in order to make them rotate around the right point.

In Limber v1.7 and above, we have allowed advanced users to modify and animate the Rotation properties of controllers, offsetting the auto-rotation produced by the expression. To enable this **Controller User Rotation** turn on the checkbox in the [settings panel](../getting-started/settings-panel.md). But be aware that if you keyframe the rotation property of an end controller, and later decide you want to use FK, those rotation keyframes won't rotate your hand or foot any more, since it'll be re-parented to the new FK controller.

{% hint style="warning" %}
If you enable Controller User Rotation and then copy and paste Rotation keyframes from one controller to another, After Effects will _also_ paste the expression along with the keyframe values, and this can cause problems. If you need to copy rotation keyframes, disable the expression beforehand, so that AE **only** copies the values and not the expression.
{% endhint %}

Some animators want to use FK but also be able to rotate the hand or foot layer with keyframes on the end controller. One way to do this is to manually add an Angle Expression Control Effect to the end controller, and expression-pickwhip the hand layer's rotation to this angle control.
