# Hii, I'm Daniel!

I like writing software! Web development, CLI tooling, libraries, it's all fun!

Knowing specs, protocols, and the problems that other tools solve lets you use them much more effectively, that's what I think anyway! Combing through docs, specs, RFCs, code, then making something with that knowledge, that's how I like to learn!

The way I see it: If I can replicate its functionality, I can probably use it quite well immediately after looking at the docs.

## Repos!
### [:cherry_blossom: blume](../../../blume)

The condensed patterns that I found after creating ~60 CLI tools, with [list](../../../list) being the most influential of them. It introduces things like predicates, has a focus on array operations and pipe-like, data-flow approach to composition, and provides very useful functions for file system operations and string manipulation.

### [:card_index_dividers: list](../../../list)

`ls`, but also like 12 other tools. It's effectively a stack based tacit left-to-right DSL for querying the file system. It's syntax allows for arbitrary number of operations to be specified. However, it remains performant, scaling well with queries as well as size of input. For example, `list` recurses, indexes, and sorts a directory of 20+ million files in under 30 seconds.

### [:spider_web: wd](../../../wd)

The experience I want to have with web development! Includes separate tools, all related to web development. Things like a simple, secure, easy to use reverse proxy (with ACME, automated DNS configuration, SNI, etc.), specifically for local-to-public hosting. A static site dev server that embeds a live reload script to html! A file server that accepts file paths from pipes, not fancy, but it works.

### [:hammer_and_wrench: tools](../../../tools)

A single repo for many small tools. These tools build an ecosystem. They have the same semantics and are very interoperable. Many of them can be thought of as CLI wrappers for [:cherry_blossom: blume](../../../blume) libraries. Has many of the classic core utils, but they're friendlier this time!


## Answers to questions no one has asked me :D

**\>Why do you use Go so much? Why not other languages?**\
<Go is nice and simple, it gives me what I need and then does everything automatically. I love JavaScript, and I use Python a lot too! But when it comes to smoothness of development, neither JS or Py have anything (that I know of) that's like [Go workspaces](https://go.dev/blog/get-familiar-with-workspaces). Go tooling is just so nice!

**\>Why try to reinvent the wheel so much? Not-Invented-Here syndrome?**\
<I feel that when you try to make things yourself you get to learn the lessons yourself. Besides, it's really fun! When the situation calls for the industry standards, those lessons learned pay dividends.

**\>Which tool you've made is your favorite?**\
[`list`](../../../list), and by a large margin. In fact, I have been using it as my `ls` for nearly a year at this point. It does what I want, the way I need it to, the way how I like it. No need for `grep`, `find`, `head`, `tail`, `xargs`, ... I can just say what I want, and it does it!

**\>Which library you've made is your favorite?**\
[`blume/clog`](../../../blume/tree/main/clog)! I always found that `fmt.Println`, `log`, etc., were awkward to use, put them where you need, remove once you don't, then do it all over again the next time a problem pops up. `clog` is a styled `log/slog` implementation, with normalizing width for rows, colored logging levels, max length for messages, etc. As it turns out, when you make good logging in a project from the start, it makes everything else easier as well!
