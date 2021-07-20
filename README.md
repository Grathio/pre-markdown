# `<pre-markdown>`

Wrap Markdown text in `<pre-markdown>` tags to render in the browser.

## Usage

In your html, include the script:

```html
<script src="path/to/pre-markdown.js"></script>
```

Then use `<pre-markdown>` tags around your Markdown text.

```markdown
<pre-markdown>
# This will display as an h1 header

This is some **bold** text, and this is *italics* in _two ways_.

- This is a list.
- List with a [link](https://duckduckgo.com/?q=commonmark)
</pre-markdown>
```

Which will render in the browser as:

---
# This will display as an h1 header

This is some **bold** text, and this is *italics* _two ways_.

- This is a list.
- List with a [link](https://duckduckgo.com/?q=commonmark)
---


### Options

Set any of the following attributes to change the default behavior. (eg `<pre-markdown html="true" linkify="true">`

All attributes are optional.

- `css` : Link to an external CSS file to apply to the Markdown block.

  - Note that an external CSS file will completely override the built-in CSS.

- `html` : Set this to render HTML tags inside the Markdown. *Default: unset. HTML is escaped.*

- `linkify` : Set this to turn link-like things into links. (web addresses, emails, etc.) *Default: unset. URLS are unchanged.*

- `typographer` : Set this to do some language-neutral replacement and make quotes pretty. *Default: unset. Quotes are unchanged.*

- `breaks` : Set this to turn newlines (`\n`) within paragraphs into `<br>` tags. *Default: Unset. Single line breaks within a paragraph are ignored.*

  

### Example:

See the `/examples/` folder for more robust usage.


## Compatibility

### Browser

Roughly speaking `pre-markdown` is compatible with any browser that is capable of the `import` syntax. [compatibility chart](https://caniuse.com/es6-module-dynamic-import) This includes virtually every browser—desktop and mobile—that has had a release since 2019.

### Markdown

`<pre-markdown>` uses the [markdown-it](https://github.com/markdown-it/markdown-it) rendering engine which follows the [CommonMark specification](https://spec.commonmark.org/). It's generally compliant and fast. Parsing uses the [markdown-it defaults](https://markdown-it.github.io/markdown-it/). See [Options](#options) above for configuration options.

## Licenses

```
pre-markdown is MIT licensed.
https://github.com/Grathio/pre-markdown
Copyright © 2020-2021 Steven Hoefer.
```

```
markdown-it is MIT licensed.
Copyright © 2014 Vitaly Puzrin, Alex Kocharin.
https://github.com/markdown-it/markdown-it
```
