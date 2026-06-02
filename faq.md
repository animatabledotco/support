---
description: >-
  This guide is no longer updated. It is for an old, outdated version of Limber
  (v1.7.5).
---

# FAQ

### Why do things go weird when I use blending?

If your FK blending seems to go the wrong way, it's worth checking the rotation values of your IK controllers: they may be 360º higher or lower than you expect.

If you are blending FK whilst the upper limb goes around North (e.g. crosses over 0º or ‘straight upwards’), an undesirable jump can occur in the position of the FK Controller. Similarly, if you animate Rotate Start / Rotate End values between 0 and 100% whilst the upper limb passes across north, their rotation will flip suddenly.  This is a limitation of our math.  The only real solution is to complete the blend before (or start it after) the point where the upper limb goes around the north axis.

Generally, try not to blend other properties whilst blending FK.  If you blend between clockwise and anti-clockwise whilst FK is neither 0 nor 100, it can produce odd jumps or flips during the animation.

Limbs on full FK are always the length given in the Length properties. They are not affected by Stretch, Anti-pop or Clockwise properties. But those properties can affect the apparent length of the limb when on IK.  So when blending between a pose where the limb is being significantly shortened by Anti-pop or Clockwise (or lengthened by Stretch), and an FK pose, it can look like the limb is changing length.  To prevent this, either reduce the effects of the length-altering property before the blend takes place, or blend at a different point in time.

### Is Limber compatible with Lottie / Bodymovin? <a href="#bodymovin" id="bodymovin"></a>

Limber's default limbs are fully compatible with Bodymovin and Lottie for web, (apart from the _Legacy Taper_ - just use a standard taper instead). Custom limbs, including those that you have rigged artwork to, may or may not work as expected - because Limber supports all Shape layer features, but Bodymovin does not.  The Merge Paths operator and Tapered Strokes, for example, are not supported in Bodymovin.

At the time of writing, Lottie for devices still does **not** support _any_ After Effects expressions, and so you will need to bake all expressions to keyframes in order to use limbs with Lottie for devices. This is a universal problem that affects all After Effects IK tools equally.  The good news is that Limber's default limbs use relatively few expressions, so baking them to expressions and optimising the resulting keyframes, is relatively simple.

You should always enable _Hidden_ and _Guide_ layers to use Limber with Bodymovin.

### Why are my controllers offset in the comp?

Limber does not support [non-square pixel aspect ratios](https://helpx.adobe.com/after-effects/using/importing-interpreting-footage-items.html#pixel_aspect_ratio_and_frame_aspect_ratio) and if you are using a comp with non-square pixels, things won't look right. Change your Pixel Aspect Ratio in Composition Settings to 'Square Pixels' to solve this.&#x20;
