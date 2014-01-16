## Restore my chromium wheel mouse setting!
The decision made in late 2012 to remove native support for the ability to adjust the wheel mouse scroll speed via a flag while starting chromium. For example:

`chromium --scroll-pixels=300`

Although at least one extension exists that will emulate this behavior, many prefer to have the native functionality restored. This patch will revert issue [#154776]([https://code.google.com/p/chromium/issues/detail?id=154776) and will re-enable scroll-pixels.

In the linked bug report above, you will see referenced [this ticket against GTK](https://bugs.launchpad.net/gtk/+bug/124440) which has been opened since Aug of 2007 and remains open.  The strategy of the chromium dev team apparently is to off load the mouse scrolling speed adjustment to a yet-to-be-developed GTK util.  Wtf?! Anyway, you may apply the patch I keep updated in this github repo until something official comes out.

## Contributors
* graysky2 (v25-v30)
* dolohow  (v31+)

## Arch linux package
[Here](https://aur.archlinux.org/packages/chromium-scroll-pixels) is an Arch PKGBUILD that mirrors that of the official [community]/chromium I maintain that has this patch enabled.

Arch users not wanting to compile on their own (it takes ~20 min on my 4.5 GHz Ivybridge), may freely use precompiled packages which I maintain on my unofficial repo: http://repo-ck.com

Thanks and enjoy.

## Contact me
I don't watch the linked tickets above on any frequent basis. Please [open an issue against this project](https://github.com/graysky2/chromium-scroll-pixels-patch/issues/new) if you're aware of an upstream change.


