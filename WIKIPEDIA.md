


# Wikipedia Markup Cheatsheet for Text with Instructions (.texti)


What's news? What's different?


Notes:  :white_check_mark: no changes.  :x: changes


## Text Formatting


### :white_check_mark: Italic / Emphasis

```
''italic text'' or
''emphasized text''
```

**Additions**. Alternative Syntax

```
_italic text_ or
*emphasized text*
```


### :white_check_mark:  Bold / Strong Emphasis

```
'''bold text''' or
'''strongly emphasized text'''
```

**Additions**. Alternative Syntax

```
__bold text__ or
**strongly emphasized text**
```

### :white_check_mark:  Italic + Bold

```
'''''italic bold text''''' or
'''''strongly emphasized emphasized text'''''
```



### :white_check_mark: Bulleted List

```
* Wikipedia
* Encyclopédie
```

**Additions**. Alternative Syntax

```
- Wikipedia
- Encyclopédie
```

```
+ Wikipedia
+ Encyclopédie
```


###  :x: Numbered List

:x: Old syntax

```
# A - Azymites
# B - Cézimbra
```

Why?

`#` (+space) is reserved / used for comments e.g. `# this is a comment`. 


:white_check_mark: New syntax:

```
1. A - Azymites
2. B - Cézimbra
```

or

```
1. A - Azymites
1. B - Cézimbra
```

Note: Use the same number to use the number as placeholder as before (will get auto-numbered).

Or use roman numberals, the alphabet, etc.

```
 I. A - Azymites
II. B - Cézimbra
```

```
a. A - Azymites
b. B - Cézimbra
```






### :white_check_mark: Headings

```
=Heading 1 Text=
==Heading 2 Text==
===Heading 3 Text===
====Heading 4 Text====
=====Heading 5 Text=====
======Heading 6 Text======
```

**Additions**. Alternative Syntax for Heading 1 and Heading 1

```
Heading 1
=========
```

```
Heading 2
---------
```


## Links

### :white_check_mark:  Internal `[[..]]`

Internal Link (to another page)

```
[[Denis Diderot]]
```

Internal Link with Different Text

```
[[Denis Diderot|Diderot]]
```


### :white_check_mark: External  `[..]`

Link to another website

```
[http://loc.gov]
[http://loc.gov Library of Congress Website]
```

**Additions**.  Alternative Syntax

```
[Library of Congress Website | http://loc.gov]
[Library of Congress Website  url=http://loc.gov]
```

- DISCUSS - make separator `|` optional - why? why not ???
- DISCUSS - keep `url=` version - why? why not???


```
[Library of Congress Website](http://loc.gov)
```

Reference style:

```
[Library of Congress Website][1]

...

[1]: http://loc.gov
```

### :x: (Inline) References

:x: Old syntax (Do NOT use).


``` text
{% raw %}
<ref>{{MerriamWebsterDictionary|markup language}}</ref>

-or-

<ref>Michael Downes. [http://www.ams.org/notices/200211/comm-downes.pdf "TEX and LATEX 2e"]</ref>

-or-

<ref>{{cite web|last=Bray|first=Tim|authorlink=Tim Bray
|url=http://www.tbray.org/ongoing/When/200x/2003/04/09/SemanticMarkup#p-1
|title=On Semantics and Markup, Taxonomy of Markup
|website=www.tbray.org/ongoing
|date=9 April 2003
|access-date=9 July 2015}}</ref>
{% endraw %}
```

Why change `<ref>` to `[^]`? 

The idea of Texti is to be format independent - that is - Texti instructions should not look
like html tags or latex commands, for example. Text with instructions tries to be "orthogonal" to html and latex.
The idea is that you can easily mix and match texti with html or latex without escaping one or the other
e.g. how do you know that `<ref>` is NOT an html tag or `<references>`? Simple, use `[^]` and `{% raw %}{{references}}{% endraw %}` 
- if it looks like a html tag it is a html tag, if it doesn't it doesn't, that's by design :-).


New (Inline) References:

``` text
{% raw %}
[^1|{{MerriamWebsterDictionary|markup language}}]

-or-

[^2|Michael Downes. [http://www.ams.org/notices/200211/comm-downes.pdf "TEX and LATEX 2e"]]

-or-

[^3|{{cite web
  |last=Bray|first=Tim|authorlink=Tim Bray
  |url=http://www.tbray.org/ongoing/When/200x/2003/04/09/SemanticMarkup#p-1
  |title=On Semantics and Markup, Taxonomy of Markup
  |website=www.tbray.org/ongoing
  |date=9 April 2003
  |access-date=9 July 2015}}]
{% endraw %}
```

Note: The number e.g. `^1` is "symbolic", that is, it's a placeholder - you can write
`^1` `^1` `^1`
as often as you like (when generated references will get auto-numbered).


Or use the refrence form or reference short form:


``` text
{% raw %}
yada yada [^1] yada yada yada [^2][^3] yada yada


^1: {{MerriamWebsterDictionary|markup language}}]
^2: Michael Downes. [http://www.ams.org/notices/200211/comm-downes.pdf "TEX and LATEX 2e"]
^3: {{cite web
  |last=Bray|first=Tim|authorlink=Tim Bray
  |url=http://www.tbray.org/ongoing/When/200x/2003/04/09/SemanticMarkup#p-1
  |title=On Semantics and Markup, Taxonomy of Markup
  |website=www.tbray.org/ongoing
  |date=9 April 2003
  |access-date=9 July 2015}}
  
-or-

yada yada [^] yada yada yada [^^][^^^] yada yada

^:  {{MerriamWebsterDictionary|markup language}}]
^^:  Michael Downes. [http://www.ams.org/notices/200211/comm-downes.pdf "TEX and LATEX 2e"]
^^^: {{cite web
  |last=Bray|first=Tim|authorlink=Tim Bray
  |url=http://www.tbray.org/ongoing/When/200x/2003/04/09/SemanticMarkup#p-1
  |title=On Semantics and Markup, Taxonomy of Markup
  |website=www.tbray.org/ongoing
  |date=9 April 2003
  |access-date=9 July 2015}}

{% endraw %}
```



### Categories, See also, etc.

As an easier alternative use meta data (back matter) for categories, see also, etc. Example:

``` text
---
Categories:
  - Markup languages
  - Formal languages
  - American inventions

See also:
  - Comparison of document markup languages
  - Curl (programming language)
  - List of markup languages
  - Markdown
  - ReStructuredText
  - Programming language
  - Style language
---
```

Using a page template, for example, you can turn your categories (automagically) into links and more.

