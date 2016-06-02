# How to create an archive of specific commits

If you need to share files and you can't just share your git repo.

```
$ git diff -z --name-only commit1~ commit2 | xargs -0 git archive --format zip --output ./out.zip HEAD
```

The -z flag tells git-diff to not translate NUL and the -0 flag tells xargs 
that the piped content contains NUL. This allows us to deal with spaces in 
path names.
