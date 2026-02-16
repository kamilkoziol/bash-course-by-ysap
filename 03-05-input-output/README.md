#### Input-output

##### read

To read from stdin use `read`. It might lead to some wierdness so just always use
```bash
read -r foo
```

- `-r` do not allow backslashes, basically raw

##### piping

With example above we can do

```bash
echo "hello" | ./input-output
```

And also `cat` but `read` only reads first line of file.

##### read all lines

To read all lines from file just put it in while

```bash
while read -r foo; do
    echo "yoyoyo $foo"
done
```

There is a gotcha - doesn't work if there is no new line :<

