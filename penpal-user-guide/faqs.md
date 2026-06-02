---
description: >-
  This guide is for an outdated version of Penpal (1.5.0) - please visit
  https://penpal.docs.animatable.co for the current user guide.
---

# FAQ's

#### When I click on Window > Extensions > Penpal, nothing happens.

Please try the following steps:

1. Download the latest [ZXP Installer](https://aescripts.com/learn/zxp-installer/) from aescripts.
2. In ZXP Installer, click on the Settings icon in the top-left. This opens a new pane which has three icons on the left hand side. Click on the bottom icon to bring up a list of CEP versions. Make sure that `Enable debugging` is checked on for CEP version 8 and above.
3. Click on OK.
4. Close and re-open the Penpal panel inside After Effects.

If this process fails to get Penpal working, please [open a support ticket](https://aescripts.com/contact/) at aescripts and we will help you directly. These installation issues are really down to Adobe but we can usually get things working in the end.

#### Why doesn't Penpal just work with the points I select in AE’s composition panel?

Two reasons: firstly, the After Effects software does not provide script developers with access to point selections, so we actually have no way of knowing which points on a path you have selected in the composition panel. Secondly, in Adobe software, it’s not possible to select only one tangent of a pair (other than when you’re dragging it around). So providing functions which operate on only one tangent require us to build our own way of selecting those individual tangents.

#### Can I make a suggestion?

Yes! We love to hear suggestions from users whether you've purchased a license or are just trying it out. The easiest way of doing this is to click the `hamburger menu > About & License… > Support`. Fill in your details and your idea and click the Open in Browser button to send that info to aescripts support, which will then forward your comments to us without disclosing your email address.

#### Why can't I move points and tangents around in Penpal?

This is something we can consider adding in a future version but would require a lot of extra work and possibly some compromises in the way selections are handled.

#### Why do multiple paths appear in strange places in the canvas?

Multiple paths sometimes look strange in Layer or Local space. This is because in After Effects, transformation properties like a shape group's Position or Anchor Point, often have a significant effect on how the raw path is displayed. With Layer and Local space, some or all of those transforms are negated. If this is a problem, try working with one path at a time, or switch to Comp space.

