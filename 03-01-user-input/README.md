#### Reading user input

##### Read command
Command to use:

```zsh
read variable
```

Options:

 - `-p` prompt, `-p "say my name"`

 You can pipe value to it, eg.: `yes | ./hello`


Regarding `help` - bash has this nice `help` zsh has total crap. However to find more about conditional expression go to:

`man zshmisc`

And search for `conditional expressions` or maybe `run-help test`.


##### Better loop

To loop over all arguments, without specifing `$1`, `$2` etc. Simply use:

```zsh
for thing in "$@"; do
    echo $thing
done
```
