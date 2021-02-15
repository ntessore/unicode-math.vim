
unicode-math
============

Vim keymap to type Unicode math symbols using TeX input sequences. The mapping
is from [unicode-math], with keymap entries adapted from
[astoff/unicode-math-input.el].


Installation
------------

Install with a package manager such as Vundle.


Usage
-----

Set the keymap:

    :set keymap=unicode-math

Then start typing a TeX command such as e.g. `\alpha`. After the leading `\`,
you should see that the cursor does not advance until the `α` character is
produced.

See the unicode-math [symbol list] for a complete list of symbols. In addition,
the following TeX commands are defined:

- superscripts: `^1`, `^2`, etc. where available
- subscripts: `_1`, `_2`, etc. where available


[unicode-math]: http://ctan.org/pkg/unicode-math
[astoff/unicode-math-input.el]: https://github.com/astoff/unicode-math-input.el
[symbol list]: http://mirrors.ctan.org/macros/unicodetex/latex/unicode-math/unimath-symbols.pdf
