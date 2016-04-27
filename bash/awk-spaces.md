# spaces in file or folder names

It's not a good idea to leave spaces in your folder or file names. If you do you may have trouble piping the output. Here's one way around it.

```bash
$ ls | awk '{print $1 " " $2}' > myfile.txt
```
