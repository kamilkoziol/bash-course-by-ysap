#### Section

To find different man pages just go

```bash
man man
```

The sections are somewhere there, at the top. 

```
1   Executable programs or shell commands
2   System calls (functions provided by the kernel)
3   Library calls (functions within program libraries)
4   Special files (usually found in /dev)
5   File formats and conventions, e.g. /etc/passwd
6   Games
7   Miscellaneous (including macro packages and conventions), e.g. man(7), groff(7), man-pages(7)
8   System administration commands (usually only for root)
9   Kernel routines [Non standard]
```

```bash
man 5 dunst
```

etc.

If we omit the section it will go 1,2,3... trying to eventually find the existing section.


Built-ins are not in man, to get the documentation check the `help`, eg. `help history`. Obviously it's bash, not zsh, for zsh it is `run-help`.


Remember to use `which` and `type`. There is `-a` option to type, that shows all from top to bottom:

```bash
❯ type -a ls  
ls is an alias for ls --color
ls is /usr/bin/ls
```

```bash
❯ type -a echo
echo is a shell builtin
echo is /usr/bin/echo
```

In above example `man help` is for `/usr/bin/echo` and `run-help` is for shell builtin.

Actually the configuration of `run-help` is a little bit unclear, apparently it should be somehow configured, I'm not gonna do it right now, come on.

To display all builtins (I don't know for what): `compgen -b`.
