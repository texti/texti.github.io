


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
- DISCUSS - keep url= version - why? why not???


```
[Library of Congress Website](http://loc.gov)
```

Reference style:

```
[Library of Congress Website][1]

...

[1]: http://loc.gov
```


