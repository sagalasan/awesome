# awesome

### Remove a directory from entire git history
```
git filter-branch --index-filter 'git rm -r --cached --ignore-unmatch DIRECTORY_NAME' --prune-empty -f -- --all
rm -rf .git/refs/original
git reflog expire --expire=now --all
git gc --aggressive --prune=now
```

## Git Tag
```
git tag -a v0.1.2 -m "v0.1.2"
git push origin v0.1.2
```
