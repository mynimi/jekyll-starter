---
lang: de #always define the language!
title: Standard Post # post title
name: sp1 # this is the identifier for multi-lang-support
subtitle: Ein klassischer Standard Post # add if you want a subtitle
tags: [standard, post] # all of the tags
description: Ein klassischer Standard Post für initium; # meta description, will be displayed at places like google
---
Das hier ist ein ganz gewöhnlicher Post.

Er ist in Markdown geschrieben, was super einfach zu lernen ist.
<!-- more -->
Man kann Bilder einfügen:

![alttext]({{ site.img_dir | prepend: site.baseurl }}/image.jpg)

Der Code dafür ist super simpel!

```markdown
{% raw %}![alttext]({{ site.img_dir | prepend: site.baseurl }}/image.jpg){% endraw %}
```

> Man kann Zitate einfügen!

> Auch welche die über
> mehrere Zeilen
> geschrieben sind

```markdown
> Man kann Zitate einfügen!

> Auch welche die über
> mehrere Zeilen
> geschrieben sind
```

Oder auch eine simple Tabelle!

heading | heading 2 | heading 3
--- | --- | ---
Bla | Bla | Bla
Bla | Bla | Bla
Bla | Bla | Bla

```md
heading | heading 2 | heading 3
--- | --- | ---
Bla | Bla | Bla
Bla | Bla | Bla
Bla | Bla | Bla
```

Dann gibt es natürlich noch Titel, Listen oder Links

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6


* normale Liste
* mit Bullets
* und so weiter

1. Nummerierte Liste
1. Zahlen spielen keine Rolle
1. Diese Liste hat immer eine 1 am Anfang im code

```md
# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6


* normale Liste
* mit Bullets
* und so weiter

1. Nummerierte Liste
1. Zahlen spielen keine Rolle
1. Diese Liste hat immer eine 1 am Anfang im code
```

[Link zu halfapx.com](http://halfapx.com) Schaut im Code so aus: `[Link zu halfapx.com](http://halfapx.com)`
