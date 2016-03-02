# mapping keys to commands in vim

Using a complicated example to demonstrate the syntax.

```
nnoremap resync :let g:i = 1 \| g/^ *"Id": \zs\d*\ze,/ s//\=g:i/ \| let g:i = g:i + 1<CR>
```

What matters is the following:

```
nnoremap resync :<CR>
```

Also note the escaping with a backslash of the pipe characters. `\|`
