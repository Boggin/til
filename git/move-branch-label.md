# move the branch label

Using git-tfs with different "branches" in TFVS doesn't let you track
the upstream. You need to move the branch label yourself after a fetch.

```
$ git branch -f branch-label SHA1
```

note: you can't be on the branch you are trying to move the label for.
