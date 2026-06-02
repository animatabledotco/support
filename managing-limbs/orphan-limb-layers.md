---
description: >-
  This guide is no longer updated. It is for an old, outdated version of Limber
  (v1.7.5).
---

# Orphaned Limb Layers

When you duplicate a limb layer using After Effects’ native _Edit>Duplicate_ command, the new copy is _orphaned_ from the limb layer set. It is still linked to the same controllers, but Limber's functions  will no longer be able to do anything with this orphaned layer. It's not part of the [set](../getting-started/controllers-and-limb-layers.md) of limber layers.

Sometimes you might need to use orphaned limb layers, and it can be useful to be able to [copy and paste](copying-and-pasting-limbs.md) them.  When you use Limber’s Copy button, Limber judges which limb layer you want to copy.  If you have a limb layer selected, that is the layer that will copy, _**even if it’s an orphaned layer**_.  But, if you have _any other_ layer selected, e.g. a controller, it will copy the style of the original, non-orphaned limb layer.  Similarly, when you paste a limb, it will only paste **to** an orphaned limb layer _if you have that layer selected_. If you have a controller selected, it will paste to the non-orphaned limb layer.

You cannot use Limber's [Replace](replacing-limbs.md) or [Duplicate](copying-and-pasting-limbs.md#duplicating) functions with orphaned limb layers. Trying to do so will result in the non-orphaned layer being replaced or duplicated instead.
