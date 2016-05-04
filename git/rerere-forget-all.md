# How to forget everything from git rerere.

Sometimes I need to start again with my merges and sometimes I'll not want what rerere remembers. 
Sometimes even `git rerere forget` isn't drastic enough. The following will clear the rerere cache:

```bash
rm -rf .git/rr-cache
```
