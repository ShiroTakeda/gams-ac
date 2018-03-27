<!--
Author: Shiro Takeda
Maintainer: Shiro Takeda
First-created: 2018-03-26.
Time-stamp: <2018-03-27 14:56:24 st>
-->

What is gams-ac.el?
============================================================

This lisp provides a auto-complete source for GAMS mode.
+ [gams-mode](https://github.com/ShiroTakeda/gams-mode).
+ [auto-complete](http://cx4a.org/software/auto-complete/).


Screenshot
============================================================

![gams-ac screenshot](gams-ac.png)


Installation
=============

First, ensure `auto-complete` and `gams-mode` are installed: I recommend
using packages from [MELPA][melpa]. 

You'll need both `auto-complete` and `slime` to be enabled and working, so
please consult the corresponding documentation is you have any trouble
with this.

Next, install `gams-ac`. If you choose not to use the convenient package
in [MELPA][melpa], you'll need to add the directory containing
`gams-ac.el` to your `load-path`, and then `(require 'gams-ac)`.

`gams-ac` provides a couple of `gams-mode`-specific completion sources, so
`auto-complete` needs to be told to use them when `gams-mode` is
active. To do this, put the following code in your emacs init file to

    (gams-ac-after-init-setup)

Usage
=====

`gams-ac` should now automatically be enabled when you visit a buffer
in which `gams-mode` is active and `auto-complete` is enabled.

If you want to add more keywords, for example, "computable", "general",
"equilibrium", Add the following into your init.el.

    (setq gams-ac-source-user-keywords
            '("computable" "general" "equilibrium"))



<!--

--------------------
Local Variables:
fill-column: 80
mode: markdown
End:

-->
