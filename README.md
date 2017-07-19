[Text with Instructions (.texti) @ GitHub](https://github.com/texti)


# Text with Instructions (.texti) - Structured Documents in Text with Formatting Conventions

_The Best of Markdown, Wikipedia Markup, LaTeX & Friends - All Together Now_



## Why? Why? Why?

Evolution vs Frozen Forever (100 % Complete)

Is the English language frozen? Is the Python or Ruby scripting
language frozen?
Is the Hypertext markup language (HTML) frozen?

Let's welcome the living language.
Let's evolve Markdown. And let's evolve Wikipedia Markup.

Use what works and don't use what doesn't work. Have we learned anything
in the last 10+ years? Anyone? Anything?

Hint: AsciiDoc? Have you heard about AsciiDoc?


### What's wrong with AsciiDoc?

The obvious ;-) a silly name, that is, text in 2020 is more than 7 or 8-bit ASCII
(American Standard Code for Information Interchange).

More serious - AsciiDoc is a new language.
Text with Instructions (.texti) is NOT a new text language -
it evolves Markdown and Wikipedia Markup, that is,
the majority (lets say 70%) is still Markdown or Wikipedia Markup
but with (lets say 20%) deletions (e.g. `..` for hard-line breaks, `![]()` for image links, etc.)
and (lets say 10%) changes (e.g. headings start with `=`, for example).



### Markdown Evolved. 10+ Years Later. Additions. Changes. Deletions.

To repeat: Have we learned anything
in the last 10+ years? Anyone? Anything?

Use what works and don't use what doesn't work.


### Let's Welcome Wikipedia Markup

A dream... One day Wikipedia Markup and Markdown evolved into
one text language. Imagine writing your Wikipedia articles
in the same text language as your notes or your next book.

A start let's change the headings to Wikipedia markup headings
`=` is the `#`
to make Wikipedians feel at home.

Next let's change page links to Wikipedia links
`[[...]]` is the new `[...]` and `[...]` gets only used for "external" links.



### What's wrong with Markdown (.md)?

The name is too clever. Markdown is a play on markup. Up and down.
Markdown is markup done right, get it? Sale! Sale! 70 % Markdown! Every Markup Tag Must Go!

The file extension is `.markdown`, `.mdown`, `.mkdn` or `.md`. Again too cryptic.

Why Text with Instructions?

The idea is that it's just text, text, text. No clever name that
hides the obvious it's just text. You have a text box?
Use text with instructions. It's just text.

The ideal file extension is `.txt` or `.text`.
More realistic and pragmatic to avoid confusion with other text formats
use `.texti` or `.txti` as the "official" Text with Instructions file
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


#### Headings marker change to Wikipedia Markup (`=` is the new `#`)

```
= Heading 1 =
== Heading 2 ==
=== Heading 3 ==
==== Heading 4 ==
===== Heading 5 ==
====== Heading 6 ==

or

=Heading 1
==Heading 2
===Heading 3
====Heading 4
=====Heading 5
======Heading 6
```

Why?

1. Let's welcome the Wikipedians. Use the headings convention from Wikipedia Markup.

2. `#` is the universal comment (in the unix world). Let's use the same comment sign
   for markdown and meta data blocks (in YAML, JSON 1.1, etc.)


More changes.

Headings are headings. Period.

You CANNOT use headings inside lists or code blocks etc. A heading always MUST start on a new line. Period.

 :x:  Old syntax (Do NOT use):

```
- ### Big ###
- ## Bigger ##
- # Biggest #
```

or

```
Paragraph
Heading
----               <-- heading 2 marker, please!?
Paragraph
```

> We should not be looking at top-level = setext headings, but second-level - ones, 
> because they're ambiguous with "thematic breaks". There are four general ways to parse this:
>
> - Paragraph, heading, paragraph
> - Heading (with 2 lines), paragraph
> - Paragraph (with 2 lines), separator, paragraph
> - Paragraph (with 4 lines)

(Source: [talk.commonmark.org/t/issues-we-must-resolve-before-1-0-release-8-remaining](https://talk.commonmark.org/t/issues-we-must-resolve-before-1-0-release-8-remaining/1287/14))


Easy rule in Text with Instructions (.texti). Setext headings MUST be followed by a blank line.

:white_check_mark: 

```
Heading 1
=========

Heading 2
---------
```

If you do NOT want to use blank lines after headings use `=` for headings e.g.:

```
=Heading 1
==Heading 2
===Heading 3
====Heading 4
=====Heading 5
======Heading 6
```

Note: Using a space between the heading and `=` is optional. Wikipedia markup uses the "compact" version without any spaces e.g. `=Markup language=` or `==Type==` etc.



#### Bold / Strong Emphasis

```
**This is bold**  or **This is a text with strong emphasis**
'''This is bold''' or '''This is a text with strong emphasis'''
```

:x:  Old syntax (Do NOT use):

```
__This is bold__ or __This is text with strong emphasis__
```

Text with Instructions (.texti) follows txt2tag and use double underlines for underline e.g.

:white_check_mark: New syntax:

```
__This is underlined__ 
```

and 

```
--This is strike-through--
```



#### Links change to Wikipedia Markup (`[[...]]` is the new `[...]`)

Why?

Markdown has no links between Markdown pages. 

- Use triple `[[[..]]]`  for intra page links also known as anchors.
- Use double `[[..]]` for page links.
- Use single `[..]` for "classic" (external) web links.

Note:

- Use `[^1 ..]` for footnotes / references
- Use `[@see ...]` for citations / references




### Additions

#### Comments, Please!

```
# This is a comment. Where's the heading?
```

A human language without comments - is that human or possible?
Let's welcome `#` (+space) for single-line comments.

Note: The comment marker is `#` must be followed by a space, that is, `#1 or #77` is just regular text.



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


Note: You can end a document with a meta data (back matter) block too. Example:

```
---
See also:
  - Comparison of document markup languages
  - Curl (programming language)
  - List of markup languages
  - Markdown
  - ReStructuredText
  - Programming language
  - Style language

Categories:
  - Markup languages
  - Formal languages
  - American inventions
---
```

If both are present (front matter and back matter) than they will get (deep) merged.




#### "Generic" Block and Inline


To be done - like in HTML - generic marker for a block (div) and inline run (span).

```
:: Note :::::::::::::::::::::::::::::

A paragraph. 

Another paragraph.

- A list item.
- Another list item.

And so on.

:::::::::::::::::::::::::::::::::::::
```

Note: Use two or more double colons (`::`) with a block type name e.g. Note, Hint, Warning, Power User Box, David Says or anything.

The type will use a "urlified" name / slug  e.g.

- Note => `note`
- Hint => `hint`
- Warning => `warning` 
- Power User Box => `power_user_box`
- David Says => `david_says`

Use two or more double colons (`::`)  to end generic marker block.

or

Unicode "pretty" version use corner brackets (add why? why not?)


DRAFT - WORK-IN-PROGESS





### Deletions

#### Image Links

:x: Old syntax (Do NOT use):

```
![](i/cover.png)
```

:white_check_mark: Use the new template syntax from Wikipedia markup:

``` text
{% raw %} 
{{ fig|cover.png }}

or

{{ img|cover.png }}
{% endraw %}
```

DRAFT - WORK-IN-PROGESS



#### Hard-line Breaks with End-of-Line Space Space (••\n)

:x: Old syntax (Do NOT use):

``` 
How doth the little crocodile••
Improve his shining tail,••
And pour the waters of the Nile••
On every golden scale!
```

:white_check_mark: Use the new hard-line break syntax (use `//` or `\\`):

``` 
How doth the little crocodile      //
Improve his shining tail,          //
And pour the waters of the Nile    //
On every golden scale!
```

Or use the new verbatim (preformatted) block with triple quotes (`"""`):

``` 
How doth the little crocodile
Improve his shining tail,
And pour the waters of the Nile
On every golden scale!
"""
``` 

or use Unicode-Text-Art (`⌜`-top left corner bracket and `⌞`-bottom left corner bracket or `⌟` bootom right corner bracket). 
(Why? Less visible and smaller than `"""`). Even works without requiring its own line for the marker.

````
⌜
How doth the little crocodile
Improve his shining tail,
And pour the waters of the Nile
On every golden scale!
⌞
``` 

````
⌜How doth the little crocodile
 Improve his shining tail,
 And pour the waters of the Nile
 On every golden scale!⌟
``` 


Note: Inside a verbatim (preformatted) block with triple quotes (`"""`)
all formatting (e.g. bold, italics, lists, footnotes, code, etc.) works as expected.



## Appendix

{% include_relative WIKIPEDIA.md %}

{% include_relative MARKDOWN.md %}


## Meta

**License**

![](https://publicdomainworks.github.io/buttons/zero88x31.png)

The Text with Instructions format
is dedicated to the public domain. Use it as you please with no restrictions whatsoever.

**Questions? Comments?**

Post them to the [wwwmake forum](http://groups.google.com/group/wwwmake). Thanks!



