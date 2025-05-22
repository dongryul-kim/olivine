
# Olivine

A simple [Zola](https://github.com/getzola/zola) theme for a personal knowledge
base. Inspired by [Obsidian](https://obsidian.md).

## Features

* Journaling
* Tags
* Knowledge graph
* Searching
* Light/dark mode
* Keyboard shortcuts
* Backlinks

## Installation

Please follow the Zola documentation on [installing and using
themes](https://www.getzola.org/documentation/themes/installing-and-using-themes/).

There is also an additional step that is specific to Olivine. Create a file a
named `content/olivine-internal-graph.md` with contents:
```
+++
title = "Graph"
template = "internal/graph.html"
+++
```
and also a file named `content/olivine-internal-sitemap.md` with contents:
```
+++
title = "Sitemap"
template = "internal/sitemap.html"
+++
```

