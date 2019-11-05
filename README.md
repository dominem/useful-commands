# useful-commands

## GIT

Grep through repo's history:

```
git grep <regexp> $(git rev-list --all)
```

Grep through file's history:

```
git grep <regexp> $(git rev-list --all -- <file>) -- <file>
```
