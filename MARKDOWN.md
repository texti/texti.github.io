# Markdown Cheatsheet for Text with Instructions (.texti)

_Fixing (Evolving) Markdown - Deletions. Yes. Deletions. Changes. Additons._


What's news? What's different?

Notes:  :white_check_mark: no changes.  :x: changes


## Text Formatting

###  Italic / Emphasis

:x: Intra-word emphasis with underscores does NOT work anymore.  

``` text
print_hello_world    <!-  just regular text
```

<!-- spelling: use italics or just italic ?? -->


Why?

Intra-word use of underscore (_) is quite common for replacing spaces in wikipedia, tags, scripts, numbers, etc.

###  Bold / Emphasis

:x: Double underscore (\_\_) alternative. Old syntax. Do NOT use:

```
This is __no longer bold__ or text with __strong emphasis__.
```

Why?

Double underscore is reserved for underline.

```
This is now __underlined__.
```

### Headings

:x: Heading marker (`#`). Old syntax. Do NOT use:

```
# Heading 1 #
## Heading 2 ##
### Heading 3 ###
#### Heading 4 ####
##### Heading 5 #####
###### Heading 6 ######
```

Headings marker change to Wikipedia Markup (`=` is the new `#`) e.g.:

```
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
- # Bigest #
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



#### "Generic" Inline Block

```
> Note:
>
```

The "old" quotation block is now a "generic" inline block e.g. in html think `div` with a class instead of `blockquote` tag.


DRAFT - WORK-IN-PROGESS


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

Or use the new verbatim (preformatted) block with triple quotes (`"""`) or (`'''`):

``` 
"""
How doth the little crocodile
Improve his shining tail,
And pour the waters of the Nile
On every golden scale!
"""
``` 

Note: Inside a verbatim (preformatted) block with triple quotes (`"""`) or (`'''`)
all formatting (e.g. bold, italics, lists, code, etc.) works as expected.










