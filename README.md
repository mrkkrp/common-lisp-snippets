# Yasnippets for Common Lisp

To use these snippets you need to install
[Yasnippet](https://github.com/capitaomorte/yasnippet) package. Once you
have Yasnippet installed, just clone this repository into your local
`snippet` directory:

```
git clone http://github.com/mrkkrp/common-lisp-snippets ~/.emacs.d/snippets/lisp-mode
```

Restart Emacs or execute command `yas-reload-all`, like this: <kbd>M-x
yas-reload-all</kbd>.

To insert a snippet, type its name and press <kbd>↹ Tab</kbd> or
<kbd>C-i</kbd>, for example:

```common-lisp
defsystem
⇒
(asdf:defsystem :system-name
  :version      "0.1.0"
  :description  "description"
  :author       "user-full-name <user-mail-address>"
  :serial       t
  :license      "GNU GPL, version 3"
  :components   ((:file "file.lisp"))
  :depends-on   (#:alexandria))

```

…you can move through the fields pressing <kbd>↹ Tab</kbd> and edit or
delete them, some fields, like `:author` try to guess their values.

As a special bonus, there are snippets to insert headers of files that
contain information about the software license, they are smart too.

Full list of snippets (it's ever growing):

* `defclass`
* `defgeneric`
* `defmacro`
* `defmethod`
* `defpackage`
* `defparameter`
* `defsystem`
* `defun`
* `defvar`
* `dolist`
* `format`
* `gnugpl` — GNU GPL 3 header
* `in-package`
* `mapcar`
* `mitlic` — MIT License header

Have fun!
