#### Conditionals

##### To compare string:

```zsh
[[ $var1 == $var2 ]]
```

```zsh
[[ $var1 != $var2]]
```

##### Check if file exists

```zsh
[[ -f filename ]]
```

##### Kinda watcher

```zsh
while [[ -f filename ]]; then
    echo "file $filename still exists"
done
```

##### true and false commands

There are `true` and `false` commands that return 0 and 1 respectively.


Always use `[[]]`, other like `[]` or `test -f file.txt` might be wierd and obsolete. I will never write some sort of ancient POSIX compliant bourn shell script so stay away from them.
