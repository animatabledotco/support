---
description: >-
  This guide is no longer updated. It is for an old, outdated version of Limber
  (v1.7.5).
---

# Duplicating, copying and pasting Limbs

### Duplicating

### <img src="../.gitbook/assets/Button_0005_Dupe.png" alt="" data-size="original">

To duplicate a limb, select any one of it's layers and click the **Duplicate** button. This will bring up a popup window that prompts you to change the first part of the layer name, with the idea that if you had named the first limb set _Right_ you could now name the duplicate limb _Left_. Custom limbs can be duplicated just like default limbs, and the limb layer will be an exact copy of the one being duplicated, including any animation.

### Copying and Pasting

### <img src="../.gitbook/assets/Button_0001_Copy.png" alt="" data-size="original"> <img src="../.gitbook/assets/Button_0006_Paste.png" alt="" data-size="original">&#x20;

Select a Limber layer, click **Copy**, then select a layer from a different limb set and click **Paste**. The pasting process works by deleting the limb layer of the destination set and replacing it with a full blown copy of the copied limb layer, then updating properties so as to link it to the destination limb’s controllers. If you've added Effects to your limb, like _Roughen Edges_ or _Turbulent Displace_, those will be copied over too.

The Limber effect [properties](../getting-started/limb-properties.md) (Lengths, Sizes, Colors etc) on the end controller are also pasted (except Clockwise and those in the FK Group).  **If you hold Alt whilst clicking Paste, the limb layer is pasted without changing those properties**. This is often what you want when copying and pasting [custom limb layers](../custom-limbs/the-limb-library.md), eg. if you’ve already set the size and color of your destination limb.

When pasting, certain layer properties such as markers, masks, opacity, switches and effects on the destination limb layer, may be lost, replaced or reset. Keyframed properties are copied using the value at the current time.  If your destination limb has keyframes on Limber properties affected by the Paste operation, the script makes a new keyframe for them at the current time.
