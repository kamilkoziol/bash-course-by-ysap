#### Basic Variables

Apprently there is a difference in bash between printing variable value with quotes and without.

```bash
[kamil@arch-home ~]$ foo="my           text"
[kamil@arch-home ~]$ echo $foo
my text
[kamil@arch-home ~]$ echo "$foo"
my           text
[kamil@arch-home ~]$ echo '$foo'
$foo
```

Doesn't seem to be an issue in zsh anyway I suppose might be useful when passing arguments idk.

Zsh version:

```zsh
❯ foo="my                     text"
❯ echo $foo      
my                     text
❯ echo "$foo"
my                     text
❯ echo '$foo'
$foo

```

Looks good to me.

You can unset with: `unset foo`

To paste to variable just use `something=$(uname -a)`
