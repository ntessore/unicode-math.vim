
unicode-math
============

Vim keymap to type Unicode math symbols using TeX input sequences. The mapping
is from [unicode-math] via [astoff/unicode-math-input.el].


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

For a more convenient way to turn the keymap on and off, add the following lines
to your `.vimrc`:

    set keymap=unicode-math
    set iminsert=0
    set imsearch=-1

You can then toggle the unicode-math keymap by pressing `<C-6>` in insert mode.

See the unicode-math [symbol list] for a list of symbols with explanations. The
[keymap](keymap/unicode-math.vim) contains a number of additions:

- standard math commands: `\ldots`, `\cdots`
- standard TeX commands: `\S`
- superscripts: `^1`, `^2`, etc. where available
- subscripts: `_1`, `_2`, etc. where available
- Greek superscripts: `^\beta`, `^\gamma`,`^\delta` ,`^\phi`, `^\chi`
- Greek subscripts: `_\beta`, `_\gamma`,`_\delta` ,`_\phi`, `_\chi`
- clockwise contour integral alias: `\ointclockwise`
- combining ring overlays for large contour integrals: `\ointring`,
  `\ointringclockwise`, `\ointringctrclockwise`

      ⌠    ⌠    ⌠
      ⎮⃘    ⎮⃙    ⎮⃚
      ⌡    ⌡    ⌡

Note that many TeX accents correspond to Unicode combining characters that go
after the symbol.  To produce e.g. `x̄`, you need to type `x\bar`.


[unicode-math]: http://ctan.org/pkg/unicode-math
[astoff/unicode-math-input.el]: https://github.com/astoff/unicode-math-input.el
[symbol list]: http://mirrors.ctan.org/macros/unicodetex/latex/unicode-math/unimath-symbols.pdf
