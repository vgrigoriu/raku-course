---
title: Default values
---

{% include menu.html %}

Both positional and named parameters can have default values. If the function has a default value for the given parameter, that parameter may be skipped when calling the function.

## Positional parameters

An example of a default value for a function with positional parameters:

```raku
sub greet($name = 'World') {
    say "Hello, $name!";
}

greet('Merinda');
greet();
```

The first call uses the name passed as the only argument and thus prints `Hello, Merinda!`. The second call uses the default value and prints `Hello, World!`.

If a function has more than one parameters, then the default values can only be used at the end of the list of them:

```raku
sub f($a, $b, $c = 42, $d = 50) { . . . } # correct
# sub f($a = 10, $b = 20, $c, $d) { . . . } # WRONG
```

## Named parameters

The same syntax is used for setting default values for named parameters:

```raku
sub greet(:$name = 'World') {
    say "Hello, $name!";
}

greet(name => 'Merinda'); # Hello, Merinda!
greet(); # Hello, World!
```

The order of the named parameters does not matter, so any of them can have default values, even the first in the list:

```raku
sub greet(:$greeting = 'Hello', :$name) {
    say "$greeting, $name!";
}

greet(name => 'Alla'); # Hello, Alla!
```

{% include nav.html %}
