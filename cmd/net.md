# map network drives

You may not see the mapped drives you expect when you are launching 
a prompt with elevated privileges when UAC is enabled.

```
net help use
net use V: \\server\folder
net use /PERSISTENT:YES
```
