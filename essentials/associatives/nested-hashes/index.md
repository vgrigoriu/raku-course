---
title: Nested hashes
---

{% include menu.html %}

Creating nested hashes is similar to creating [nested arrays](/essentials/positionals/nested-arrays). Use curly braces to embrace the inner hashes.

```raku
my %people =
    John => {
        age => 20,
        city => 'Madrid'
    },
    Alla => {
        age => 21,
        city => 'Tokyo'
    };
```

Note that a trailing comma is a valid syntax element:

```raku
my %people =
    John => {
        age => 20,
        city => 'Madrid',
    },
    Alla => {
        age => 21,
        city => 'Tokyo',
    };
```

Having a comma helps when you edit the structure by copying and pasting the lines.

To get the elements from the inner hashes, use two keys one after another.

```raku
say %people<John><city>; # Madrid
say %people<Alla><city>; # Tokyo
```

{% include nav.html %}
