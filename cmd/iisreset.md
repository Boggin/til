# iisreset for Windows 10

`iisreset` used to be the way to refresh your web server but
that's not the case for W10.

```
$ net stop was /y && net start w3svc
```
