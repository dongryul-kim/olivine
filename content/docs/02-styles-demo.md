+++
title = "Styles demo"
taxonomies.tags = ["markdown"]
+++

This page shows the basic styles and features of the theme.

## Text

There are the standard *italic* and **strong** and ***italic strong*** fonts.
There is also ~~strikethrough~~.

## Sections (h2) {#sections-h2}

The table of contents appear in the right sidebar (expanded and folded using the
book icon). Here are some lower-level sections.

### This is a subsection (h3)

Some random text in a subsection

#### This is a subsubsection (h4)

Some other random text in a subsubsection. Anything below this is probably not
that useful.

---

We can also insert a break line.

## Lists and links

Here are some numbered and bulleted lists.

* A first bullet item
* A second bullet item
  * A first nested bullet item
  * A second nested bullet item
    * A first nested nested bullet item
  * A third nested bullet item

Links can be created using the Markdown syntax `[link name](link url)`.

1. Here is an external link to the 
   [Github repository](https://github.com/dongryul-kim/olivine).
1. Here is an internal link to [documentation page](@/docs/_index.md).
1. We can also link to sections like [Sections](#sections-h2), which is the
   previous section.

Items in lists can have checkboxes.

1. [X] Write this todo list.
1. [ ] Some big project that has multiple tasks.
   * [ ] This is not finished.
   * [X] This is finished.

## Tables and images

Here are some physical properties of minerals.

| Mineral | Chemical composition | Melting temperature |
|:-:|:-:|:-:|
| Olivine | (Mg,Fe)&#8322;SiO&#8324; | 1200--1900&#8451; |
| Obsidian | SiO&#8322;, MgO, Fe&#8323;O&#8324; | 700--900&#8451; |

In Markdown, an image is an `<img>` tag with surrounding text. For example, ![An
image of
olivine](https://upload.wikimedia.org/wikipedia/commons/f/fb/Olivine-gem7-10a.jpg)
can be part of a sentence.

## Code and math

Both inline code `sudo rm -rf /` as well as (syntax-colored) block code
```c
int fibonacci(int n) {
    if (n = 0) return 0;
    if (n = 1) return 1;
    return fibonacci(n-1) + fibonacci(n-2);
}
```
are supported. We can also include line numbers and highlight lines
```c,linenos,hl_lines=2-3
int fibonacci(int n) {
    if (n = 0) return 0;
    if (n = 1) return 1;
    return fibonacci(n-1) + fibonacci(n-2);
}
```
by adding in the options `linenos` and `hl_lines`.

Inline math such as $a^2 + b^2 = c^2$ can be used, and there are also
displayed equations
$$ \Theta \colon \mathbf{Sh}(\mathsf{G}, \mathsf{X})_ E^\lozenge
\times_{\mathrm{Bun}_ G} \mathrm{Gr}_ {G,\lbrace \mu^{-1} \rbrace,E} \to
\mathbf{Sh}(\mathsf{G}, \mathsf{X})_ E^\lozenge. $$
However, to use this feature, the `config.extra.olivine.mathjax` option needs to
be enabled.

## Blockquotes and footnotes

The following is a quote from Alexander Grothendieck's *R&eacute;coltes et
semailles*.

> The unknown thing to be known appeared to me as some stretch of earth or hard
> marl, resisting penetration... the sea advances insensibly in silence, nothing
> seems to happen, nothing moves, the water is so far off you hardly hear it...
> yet it finally surrounds the resistant substance.

Here is a footnote[^1] to a text. As you can see, footnotes can be placed
anywhere[^2] in the document.

[^1]: This footnote is at the end of the section, but it can also go at the
    bottom of the document.

## Tags

There is also a feature of creating a link to a tag. {{tag(name="olivine")}}
Note that this is a one-sided link, meaning that including this link does not
make this page have this tag. This is implemented as a shortcode.
```
{{/* tag(name="olivine") */}}
```
To add the tag to a page, use the option `taxonomies.tags` in the frontmatter.
For example, the frontmatter for this page includes the following line.
```
taxonomies.tags = ["markdown"]
```

## Admonition blocks

A `<div>` element with class `olivine-admonish` is styled to be inside a bubble.

<div class="olivine-admonish">

**Remark.** One way to create an admonition block is to write raw HTML in your
markdown file. A better way is to write a simple shortcode that does for you.

</div>

At this point, it doesn't come with fancy headers or icons.


[^2]: This footnote is at the bottom of the document. It is from the
    [Blockquotes and footnotes](#blockquotes-and-footnotes) section.
