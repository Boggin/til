# How to forget a recorded resolution in git

If you recorded a bad fix for a conflict you can tell git to forget that bad resolution:

```
git rerere forget your_file.txt
```

Afterwards, the badly resolved file will still be in your working directory. To get it back with confict markers, say:

```
git checkout --merge your_file.txt
```

Resolve the conflict again.
