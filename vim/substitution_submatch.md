# use a submatch in a substitution.

Select a submatch for a substitution with `\zs` to `\ze`. The following with replace the number in the string.

```
g/^"Year": \zs\d*\ze/ s//2016/
```
