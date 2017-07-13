# Merge project A into project B

```
$ cd path/to/project-b
$ git remote add project-a path/to/project-a
$ git fetch project-a
$ git merge --allow-unrelated-histories project-a/master
$ git remote remove project-a
```
