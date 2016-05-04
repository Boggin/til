# spaces in file or folder names

It's not a good idea to leave spaces in your folder or file names. If you do you may have trouble piping the output. Here's one way around it.

```bash
$ ls | awk '{print $1 " " $2}' > myfile.txt
```

If there are more spaces in sub folder names and you wish to pipe the results to, for instance, `xargs rm`, then you should pipe through `sed` as well.

```bash
$ find . -name '*.orig' | awk '{print $1 " " $2 " " $3}' | sed s/\ /\\\\\ / | xargs rm -rf
```
