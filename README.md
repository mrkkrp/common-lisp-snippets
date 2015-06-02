# Yasnippets for Common Lisp

[![License GPL 3](https://img.shields.io/badge/license-GPL_3-green.svg)](http://www.gnu.org/licenses/gpl-3.0.txt)
[![MELPA](http://melpa.org/packages/common-lisp-snippets-badge.svg)](http://melpa.org/#/common-lisp-snippets)

This is a collection of Yasnippets for Common Lisp. It mainly includes
snippets for top-level forms and (as a bonus) headers for popular
free-software licenses: GNU GPL and MIT License.

## Installation

To use these snippets you need to install
[Yasnippet](https://github.com/capitaomorte/yasnippet) package. Once you
have Yasnippet installed, place contents of this repository on your load
path, so Emacs can see it and add the following to your configuration file:

```
(require 'common-lisp-snippets)
```

It's now available via MELPA: <kbd>M-x package-install RET
common-lisp-snippets RET</kbd> — and you are done!

## Usage

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
delete them, some fields, like `:author` try to guess their values. Also,
snippets are especially useful when learning some language ;-)

As a special bonus, there are snippets to insert headers of files that
contain information about the software license (`gnugpl` and `mitlic`), they
are smart too.

## Contributions

Yes, please contribute! There are some stylistic conventions:

1. Name files without any extensions;

2. Start every file with this preamble:

   ```
   # -*- mode: snippet -*-
   # contributor: your name
   # name: readable name of the snippet
   # key: what user needs to enter
   # --
   ```

   The first line is needed to activate mode for snippet editing in Emacs,
   Yasnippet ships with it.

3. Make sure your files don't have empty line at the end. This is important,
   because it will be inserted too when your snippet is
   expanded. `snippet-mode` takes care of this, setting
   `require-finall-newline` to `nil`, just make sure you haven't put it
   there manually.

## License

Copyright © 2015 Mark Karpov

Distributed under GNU GPL, version 3.
