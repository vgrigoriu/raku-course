---
title: 'Exercise: Replace with antonyms'
---

{% include menu.html %}

## Problem

Create a program that replaces all the words from the command line with their antonyms. If the word is missing in the dictionary, do not modify it and print as-is.

Use a hard-coded hash to keep the dictionary of antonyms. For your convenience, here is a prepared list of about 200 pairs that you can directly copy and paste into your program: [dictionary.raku](https://github.com/ash/raku-course/blob/master/essentials/associatives/exercises/replace-with-antonyms/dictionary.raku). All the pairs are kept in both directions, e.g.:

```raku
my %dictionary =
    'above' => 'below',
    'absent' => 'present',
    # . . .
    'below' => 'above',
    # . . .
    'present' => 'absent',
    # . . .
;
```

Make the program as simple as possible and print the words line by line.

## Example

Run the program and pass a few words to it. Make sure that at least some of the words can be found in the dictionary.

```console
$ raku replace-with-antonyms.raku a quiet teacher wants to buy some salt
a
noisy
student
wants
to
sell
some
sugar
```

## Solution

✅ [See the solution](solution)

{% include nav.html %}
