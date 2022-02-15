---
title: Arcane
---

# arcane

Arcane is a modern homepage inspired by the classic web iconography.

## Contents

- [Installation](#installation)
- [Features](#features)
  - [Blog](#blog)
  - [Navigation](#navigation)
  - [Taxonomies](#taxonomies)
- [Options](#options)
  - [Author](#author)
  - [Formats](#formats)
    - [Date](#date)
  - [Socials](#socials)

## Installation

First download this theme to your `themes` directory:

```bash
cd themes
git clone https://github.com/zakharykaplan/arcane.git
```

and then enable it in your `config.toml`:

```toml
theme = "arcane"
```

## Features

### Blog

To enable the blog, you must create a blog directory, for example in
`content/blog/_index.md`, as follows:

```
+++
paginate_by = 10
sort_by = "date"
template = "blog.html"
+++
```

This requires posts to be placed within the blog directory and to enable
pagination.

### Navigation

Arcane will automatically populate the navigation menu bar with your pages,
posts, co-located assets, taxonomies (if enabled; see below).

### Taxonomies

The theme optionally supports authors, tags, and categories taxonomies enabled
in your `config.toml`:

```toml
taxonomies = [
    # You can enable/disable RSS
    { name = "authors", feed = true },
    { name = "categories", feed = true },
    { name = "tags", feed = true },
]
```

If you want to paginate taxonomies pages, you will need to overwrite the
templates as it only works for non-paginated taxonomies by default.

## Options

### Author

You can set this on a per page basis or in the [config](config.toml) file.

```toml
[extra]
author = "Zakhary Kaplan"
```

In a page (wrap this in +++):

```toml
title = "..."
date = 1970-01-01

[taxonomies]
authors = ["Zakhary Kaplan"]
```

### Formats

Certain formats within the theme can be configured in the [config](config.toml)
file.

#### Date

```toml
[extra.format]
date = "%d %b, %Y"
```

### Socials

If you want to display social links within the footer, you can define them
within the [config](config.toml) file.

```toml
[[extra.social]]
platform = "github"
url = "https://github.com/zakharykaplan"
icon = "fa-brands fa-github"
```
