## During a rebase I want to take the server version.

```
git checkout --ours -- [file]
git add  
git rebase --skip  
```

Take all of the server version:

```
git rebase <branch> -s recursive -X ours
```

__Note__: Remember that your code becomes the 'remote' and the server version becomes the 'local'.
