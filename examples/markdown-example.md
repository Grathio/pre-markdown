Loading external Markdown
=========================

This is a stand-alone Markdown document
---------------------------------------

See: `/examples/markdown-example.md`

This file is embedded in the page using the tag:
```
<pre-markdown src="markdown-example.md"></pre-markdown>
```

By default, paragraphs are separated
by a blank line. Set `breaks="true"` to
break paragraphs at any newline.


Text attributes _italic_,
**bold**, `monospace`. You can also use *single asterisks* for italic text.
***Triple asterisks*** for bold, italic.

Horizontal rule:

---

Strikethrough:
~~strikethrough~~

Bullet list:

  * apples
  * oranges
  * pears

Numbered list:

  1. lather
  2. rinse
  3. repeat

An [example link](http://example.com).

![Image](https://via.placeholder.com/350x150 "Image example")

> A block of blockquotes which uses > characters
> at the beginning of each line to indent.
> > Blockquotes can be nested.
