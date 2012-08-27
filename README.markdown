Overview
=========
Utilities for Unicode characters in Emacs.

ucs-utils
---------
This library provides some utilities for manipulating Unicode
characters.  There are three interactive commands

	ucs-utils-ucs-insert'       ; ucs-insert workalike using ido-completing-read
	ucs-utils-eval'             ; the inverse of ucs-insert
	ucs-utils-install-aliases'  ; install shorter aliases

 The other functions are only useful from other Lisp code:

	ucs-utils-char
	ucs-utils-first-existing-char
	ucs-utils-vector
	ucs-utils-string
	ucs-utils-intact-string
	ucs-utils-pretty-name
	ucs-utils-read-char-by-name
	ucs-utils-subst-char-in-region


A typical use might be

	(setq bullet-char (ucs-utils-char "Bullet Operator" ?. 'cdp))

See Also
---------
M-x customize-group RET ucs-utils RET

[http://en.wikipedia.org/wiki/Universal_Character_Set](http://en.wikipedia.org/wiki/Universal_Character_Set)

Compatibility and Requirements
------------------------------
Tested only on GNU Emacs version 24.1

Requires persistent-soft.el

Uses if present: memoize.el
