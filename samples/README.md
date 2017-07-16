# Text with Instructions (.texti) Samples


## Article - Markup language

.texti Source:

- [samples/Markup_language.texti](Markup_language.texti)

(Auto-)Generated Formats:

- [samples/Markup_language.md.txt](Markup_language.md.txt) - Markdown
- [samples/Markup_language.latex](Markup_language.latex) - LaTeX
- [samples/Markup_language.html](Markup_language.html) - Hypertext Markup Language (HTML)


(Source: [Markup language @ Wikipedia](https://en.wikipedia.org/wiki/Markup_language),
[Wikimedia Markup Source Text](https://en.wikipedia.org/w/index.php?title=Markup_language&action=raw))


### What's different?

_Text with Instructions (.texti) Compared to Wikipedia Markup)_


**(Inline) References**

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

Note: The number (`^1`) is "symbolic", that is, it's a placeholder - you can write
`^1` `^1` `^1`
as often as you like (when generated references will get auto-numbered).


vs

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


**Inline Code**

``` text
An example of descriptive markup would be HTML's `<cite>` tag.

-or-

The codes `h1`, `p`, and `em` are examples of semantic markup.
```

vs

``` text
An example of descriptive markup would be HTML's <code>&lt;cite></code> tag.

-or-

The codes <code>h1</code>, <code>p</code>, and <code>em</code> are examples of semantic markup.
```
