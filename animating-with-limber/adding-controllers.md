---
description: >-
  This guide is no longer updated. It is for an old, outdated version of Limber
  (v1.7.5).
---

# Adding controllers

### FK Controllers

### <img src="../.gitbook/assets/Button_0011_FK.png" alt="" data-size="original">&#x20;

If you have a hand or foot layer parented to the end controller, that layer won't follow the end of the limb when you dial up FK. The solution is to click **Add FK** to generate a new **FK controller**, and parent your hand or foot to this layer instead. If you make sure the FK is set to zero before you click Add FK, Limber automatically does the re-parenting for you.

FK controllers are also useful as non-stretchy end controllers. If you have the [Stretch](../getting-started/limb-properties.md#dynamics) property _unchecked_, and you have a foot layer parented to your IK end controller, your foot can be detached away from the end of the limb when it's over-stretched. Use an FK controller to limit it to the limb length.

### Joint Controllers

### <img src="../.gitbook/assets/Button_0010_Joint.png" alt="" data-size="original">&#x20;

Joint controllers follow the position of the limb joint, should you need something to parent knee or elbow artwork to. The Joint controller has it's own Limber Joint effect on it with four rotation options. **None** will make the controller always point downwards at 0º.  **Outwards** will align the controller to the direction the joint itself points towards.  **With Lower** will aim it towards the end controller, and **With Upper** will aim it directly away from the Start Controller.  With Lower and With Upper rotations do not respond to Bone Curvature values, they behave as if the limb were two, straight sections.

{% hint style="info" %}
FK controllers and Joint controllers are never keyframed or positioned by the user. They are only there for when you need a layer to parent things to.
{% endhint %}

### Removing controllers

**You cannot remove FK and Joint controllers by simply deleting them**.  Instead, you'll need to **Alt**-click on the respective Add button, with one or more layers from the set selected.  If you remove an FK Controller when FK is set to zero, Limber will automatically re-parent any child layers to the relevant end controller.
