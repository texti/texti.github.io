[Text with Instructions (.texti) @ GitHub](https://github.com/texti)


# Text with Instructions (.texti) - Structured Documents in Text with Formatting Conventions

_The Best of Markdown, Wikipedia Markup, LaTeX & Friends - All Together Now_



## Why? Why? Why?

Evolution vs Frozen Forever (100 % Complete)

Is the English language frozen? Is the Python or Ruby scripting
language frozen?
Is the Hypertext markup language (HTML) frozen?

Let's welcome the the living language.
Let's evolve Markdown. And let's evolve Wikitext.

Use what works and don't use what doesn't work. Have we learned anything
in the last 10+ years? Anyone? Anything?

Hint: AsciiDoc? Have you heard about AsciiDoc?


### What's wrong with AsciiDoc?

The obvious ;-) a silly name, that is, text in 2020 is more than 7 or 8-bit ASCII
(American Standard Code for Information Interchange).

More serious - AsciiDoc is a new language.
Text with Instructions (.texti) is NOT a new text language -
it evolves Markdown and Wikitext, that is,
the majority (lets say 70%) is still Markdown
but with (lets say 20%) deletions (e.g. `..` for hard-line breaks, `![]()` for image links, etc.)
and (lets say 10%) changes (e.g. headings with `=`, for example).



### Markdown Evolved. 10+ Years Later. Additions. Changes. Deletions.

To repeat: Have we learned anything
in the last 10+ years? Anyone? Anything?

Use what works and don't use what doesn't work.


### Let's Welcome Wikitext (Wikipedia's Markup Language

A dream... One day Wikitext and Markdown evolved into
one text language. Imagine writing your Wikipedia articles
in the same text language as your notes.

A start let's change the headings to Wikitext headings
`=` is the `#`
to make Wikitext feel at home.

Next let's change links to Wikitext links
`[[...]]` is the new `[...]`



### What's wrong with Markdown (.md)?

The name is too clever. Markdown is a play on markup. Up and down.
Markdown is markup done right, get it? Sale! Sale! 70 % Markdown! Every Markup Tag Must Go!

The file extension is .markdown or .mkdwn or .md.
Again too cryptic.

Why Text with Instructions?

The idea is that it's just text, text, text. No clever name that
hides the obvious it's just text. You have a text box?
Use text with instructions. It's just text.

The ideal file extension is .txt or .text.
More realistic and pragmatic to avoid confusion with other text formats
use .texti or .txti as the "official" Text with Instructions reserved file
extensions.

Again the idea is that it's just text.




### What about CommonMark?

CommonMark is great. It has different
goals for the evolution of Markdown than Text with Instructions.

The goal of CommonMark is a strictly specified Markdown
with hundreds of collected verifable test cases.
That's great. Must I use a space between the heading marker `#`
and the text? Must I use blank line before a heading?
And so on.

Text with Instructions evolves Markdown, that is,
Deletions. Yes. Deletions. Changes. Additions.




## Evolutions


### Changes


#### Headings marker change to Wikitext (`=` is the new `#`)

```
= Heading 1 =
== Heading 2 ==
=== Heading 3 ==
==== Heading 4 ==
===== Heading 5 ==
====== Heading 6 ==

or

= Heading 1
== Heading 2
=== Heading 3
==== Heading 4
===== Heading 5
====== Heading 6
```

Why?

1. Let's welcome the Wikipedia. Use the headings convention from Wikitext.

2. `#` is the universal comment (in the unix world). Let's use the same comment sign
   for markdown and meta data blocks (in YAML, JSON 1.1, etc.)



#### Links change to Wikitext (`[[...]]` is the new `[...]`)

Why?

Markdown has no links between Markdown pages.


#### "Generic" Inline Block

```
> Note:
>
```

The "old" quotation block is now a "generic" inline block.






### Additions

#### Comments, Please!

```
# This is a comment. Where's the heading?
```

A human language without comments - is that human or possible?
Let's welcome `#` for single-line comments.




#### Meta Data Blocks

You can start a document with a meta data (front matter) block. Example:

```
---
# this is a meta data block
# this is a comment in the meta data block

...
---

# this is a comment in the text body

== Heading 2 ==

=== Heading 3 ===
```




#### "Generic" Block and Inline


To be done - like in HTML - generic marker for a block (div) and inline run (span).





### Deletions

#### Image Links

```
![](i/cover.png)
```

Use the new link syntax.



#### Hard-line Breaks with End-of-Line Space Space (••\n)

```
How doth the little crocodile••
Improve his shining tail,••
And pour the water
ale!
```

Use the new hard-line break syntax.




## Meta


## Meta

**License**

![](https://publicdomainworks.github.io/buttons/zero88x31.png)

The Text with Instructions format
is dedicated to the public domain. Use it as you please with no restrictions whatsoever.

**Questions? Comments?**

Post them to the [wwwmake forum](http://groups.google.com/group/wwwmake). Thanks!



