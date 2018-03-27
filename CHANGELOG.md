<!--
Author: Shiro Takeda
Maintainer: Shiro Takeda
First-created: 2018-03-26.
Time-stamp: <2018-03-27 14:55:00 st>
-->

----------------------------------------------------

Change logs of gams-ac.el
====================================================

Version 0.9 (2018-03-26)
----------------------------------

* Added hook variables `gams-sil-mode-hook`, `gams-lxi-mode-hook`, and
  `gams-ol-mode-hook`.

* Added new list code "gams-auto-complete.el". This enables you to use
  auto-complete mode in GAMS mode.

  If you want to use auto-complete mode in GAMS mode, you first need to
  install "auto-complete.el" which can be installed from MELPA.

  To use auto-complete in GAMS mode, add the following code to init.el.

        ;; Load gams-auto-complete.
        (require 'gams-ac)
        ;; Initial setup for auto-complete in GAMS mode.
        (gams-ac-after-init-setup)

  If you want to add words for auto-complete mode by yourself, add words
  to the variable `gams-ac-source-user-keywords-list`. See
  "gams-setting-sample.el" for details.






--------------------
Local Variables:
mode: markdown
fill-column: 80
coding: utf-8-dos
End:
