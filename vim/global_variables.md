# create a global variable for macros

A global variable can be used in a vim macro.

```
:let g:i = 1 \| g/^ *"Id": \zs\d*\ze,/ s//\=g:i/ \| let g:i = g:i + 1
```

The use of the `g:` lets us set `i` to a number. The use of the equals sign (escaped), `\=`, lets us retrieve its value.
