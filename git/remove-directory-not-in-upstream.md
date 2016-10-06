# git-tfs has folders that don't exist in TFVS

TFS can be funny about how folders get removed and git-tfs can end up with
folders that don't exist upstream. You can't commit the deletes as they
don't exist. `filter-branch` after ignoring.

```
$ git update-index --assume-unchanged ./folder/sub-folder/
$ git filter-branch -f --tree-filter 'rm -rf ./folder/sub-folder/'
```
