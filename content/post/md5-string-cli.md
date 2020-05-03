+++
title = "Generate MD5 hash of a string on the Terminal"
description = "While working on a [Gravatar](https://en.gravatar.com/) integration. I needed to generate a md5 hash…"
date = 2020-05-03
tags = ["til", "md5 hash", "cli", "linux"]
categories = ["TIL"]
menu = ""
banner = ""
images = []

draft = false
+++

While working on a [Gravatar](https://en.gravatar.com/) integration. I needed
to generate a md5 hash of the test email address. Surprisingly enough, this was
not as intuitiv as I though it would be. Keeping a reference here for my future
self:

```sh
$ echo -n "myemailadress@example.com" | md5sum
```

Reference:
- https://askubuntu.com/a/53852

[modeline]: # ( vim: set  tw=120 spell spl=en: )
