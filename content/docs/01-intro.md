+++
title = "Getting started"
taxonomies.tags = ["olivine"]
+++

To get started, follow the instructions below.

## Installing Zola

Check out the Zola project website for instructions on installing it.

* [Github repository](https://github.com/getzola/zola)
* [Zola documentation](https://www.getzola.org/)
* [Tera documentation](https://keats.github.io/tera/)
* [Zola community forum](https://zola.discourse.group/)

## Installing Olivine

You can use either clone a template repository or manually set up the theme.

### Option 1: template repository

Simply clone the template repository.

```bash
$ git clone git@github.com:dongryul-kim/olivine-template.git <your-folder-name>
```

### Option 2: manual configuration

There is a page in the Zola documentation on [installing and using
themes](https://www.getzola.org/documentation/themes/installing-and-using-themes/).

```bash
$ mkdir <your-folder-name>
$ cd <your-folder-name>
$ zola init
$ git clone git@github.com:dongryul-kim/olivine.git themes/olivine
# Add the option theme = "olivine" to config.toml
$ zola serve
# Navigate to localhost:1111 on the web browser
```

Because of some limitations, there are additional steps one has to take. Create
a file a named `content/olivine-internal-graph.md` with contents
```
+++
title = "Graph"
template = "internal/graph.html"
+++
```
and also a file named `content/olivine-internal-sitemap.md` with contents
```
+++
title = "Sitemap"
template = "internal/sitemap.html"
+++
```

