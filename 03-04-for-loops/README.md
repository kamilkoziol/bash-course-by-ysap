#### For loops

##### Range

It is possible to use range in for loops via `{a..f}`. It includes on both sides.
Same with numbers : `{1..7}`

It just expands to `1 2 3 4 5 6 7` so i guess i can use it in any other place. 
However we can use `{1..$max}` which replaces max but doesnt recognize the `{}` pattern.

##### C style

For max syntax we can use c style:

```bash
for ((i = 0; i < max; i++)); do
done

```

Double (()) are some sort of math mode so we don't need dollar sign before max variable name.
