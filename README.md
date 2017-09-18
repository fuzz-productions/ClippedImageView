Auto-masking Views for Android
==============================

These custom ImageViews use their backgrounds as masks to clip their
foregrounds. Many libraries limit themselves to just a couple of simple
shapes: circles, ovals, squircles, teardrops, and (of course) rectangles.

With this, you can use _any_ transparency-sporting drawable as a mask -
even vector assets!

The code used for this library was derived from work by @fanrunqi on
their [AvatarImageView][0].

Prior to 9/2017 these files were shipped as part of [CutoutViewIndicator][1]

Who would use this?
-------------------
This library is aimed at any android app loading images into
ImageViews (or ImageButtons, etc...). We support all the big image-loading
libraries (Glide, Picasso, Volley) as well as standard Android framework
methods (`android:src`, `setImageDrawable`, `app:srcCompat`).

So, uh, what do clipping and masking even mean? in this context?
----------------------------------------------------------------
Clipping is the act of removing all visible parts of an image outside a
certain boundary. That boundary is usually called the 'clip bounds', and
an image made up entirely of area outside the clip bounds is called a 'mask'.

# License
```
Copyright 2016 fanrunqi

Modifications Copyright 2016-2017 Philip Cohn-Cort

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

 [0]: https://github.com/fanrunqi/AvatarImageView
 [1]: https://github.com/fuzz-productions/CutoutViewIndicator
