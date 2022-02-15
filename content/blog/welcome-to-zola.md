---
date: 2022-01-01
template: post.html
title: Welcome to Zola
taxonomies:
  authors:
    - Zakhary Kaplan
  categories: [meta]
  tags: [welcome, zola]
---

You’ll find this post in your `content/blog` directory. Go ahead and edit it and re-build the site to see your changes.
You can rebuild the site in many different ways, but the most common way is to run `zola serve`, which launches a web server and auto-regenerates your site when a file is updated.

<!-- more -->

To add new posts, simply add a file in the `content/blog` directory includes the necessary front matter.
You could also optionally start a filename with a datetime (YYYY-mm-dd or [an RFC3339 datetime](https://www.ietf.org/rfc/rfc3339.txt)) followed by an underscore (`_`) or a dash (`-`) will use that date as the page date, unless already set in the front matter.
Take a look at the source for this post to get an idea about how it works.

Zola also offers powerful support for code snippets:

```rust
let print_hi = |name| {
    println!("Hi, {name}");
};
print_hi("Zak");
// prints "Hi, Zak" to `stdout`.
```

Check out the [Zola docs][zola-docs] for more info on how to get the most out of Zola. File all bugs/feature requests at [Zola’s GitHub repo][zola-github].
If you have questions, you can ask them on the [Zola Forum][zola-forum].

[zola-docs]:   https://www.getzola.org/documentation
[zola-github]: https://github.com/getzola/zola
[zola-forum]:  https://zola.discourse.group
