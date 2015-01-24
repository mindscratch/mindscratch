craigwickesser.com
===

This is the code behind the site [craigwickesser.com](http://craigwickesser.com), used by
[Hugo](http://hugo.spf13.com) to generate a static html site.

This site was forked from [npf.io](http://npf.io), thanks for some interesting
ideas (i.e. series) and styling.

### How to create a series?

Create a new file under `content/desc` named `series-<name>md`, such as
`series-golang-for-beginners.md`. It should look like this:

```
+++
Description = ""
date = 2015-01-23T21:22:48Z
title = "series golang-for-beginners"
series-desc = ["Go for Beginners"]
+++

Go for Beginners is a series of posts to get developers started with Go.
```

### How to add code pages?

To add a page for a code related project, add a file in `content/code`, such
as `content/code/foo.md`:

```
+++
date = "2015-01-23T21:30:14-05:00"
title = "foo"
menu = "code"
repo = "foo"
pkg = "foo"
norss = true

[[badges]]
alt = "godoc"
img = "https://godoc.org/mindscratch/foo?status.svg"
url = "https://godoc.org/mindscratch/foo"
+++

Foo is a Go library for doing nothing.

The code is hosted at https://github.com/mindscratch/foo but the import path is
"craigwickesser.com/foo" and the package name is keep.
