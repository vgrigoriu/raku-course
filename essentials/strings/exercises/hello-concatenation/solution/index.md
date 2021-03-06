---
title: Solution to ’Hello, Concatenation!‘
---

{% include menu.html %}

## Code

Here is a possible solution to this problem:

```raku
my $name = prompt 'What is your name? ';
say 'Hello, ' ~ $name ~ '!';
```

🦋 You can find the source code in the file [hello-concatenation.raku](https://github.com/ash/raku-course/blob/master/exercises/strings/hello-concatenation.raku).

## Output

Run the program, and it will enter a mode when it waits for your input. After you type the name and press Enter, the program goes on and prints the greeting:

```console
$ raku exercises/strings/hello-concatenation.raku
What is your name? John
Hello, John!
```

## Comments

Compare the program with [the previous variant](../../../../scalar-variables/exercises/greet-a-person/solution) where we passed three strings to the `say` routine:

```raku
say 'Hello, ', $name, '!';
```

This time, the three parts are first concatenated and then passed to `say` as a single string.

{% include nav.html %}
