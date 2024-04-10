+++
title = "Styles demo"
+++

This page shows the basic styles and features of the theme.

## Text demo

The above section is a `<h2>` element. Here are some lower-level sections.

### This is a subsection

Some random text inside the `<h3>` element.

#### This is a subsubsection

Some other random text inside the `<h4>` element. Anything below this is not
very useful in my opinion.

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
1. We can also link to sections like [Text demo](#text-demo), which is this
   section.

There is also a feature of creating a link to a tag. {{tag(name="olivine")}}
Note that this is a one-sided link, meaning that including this link does not
make this page have this tag. This is implemented as a shortcode.
```
{{/* tag(name="olivine") */}}
```

## Tables and images

Here are some physical properties of minerals.

| Mineral | Chemical composition | Melting temperature |
|:-:|:-:|:-:|
| Olivine | (Mg,Fe)&#8322;SiO&#8324; | 1200--1900&#8451; |
| Obsidian | SiO&#8322;, MgO, Fe&#8323;O&#8324; | 700--900&#8451; |

