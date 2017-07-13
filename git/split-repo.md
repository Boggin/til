# Split repository up

```
$ git clone <repo> new_dir
$ cd new_dir
$ git filter-branch --prune-empty --subdirectory-filter <sub-folder> master
```
