
### Make an empty commit to trigger build.

```sh
git commit --allow-empty -m "Trigger build"
```

### Undo last commit

```sh
git reset --soft HEAD~1
```

### Reset file changes with base branch

```sh
git checkout origin/main -- src/transformers/response.transformer.ts
```

### Delete All Local Branches (except current and protected)

```sh
git branch | grep -v "\*\|main\|master\|develop" | xargs -n 1 git branch -D
```

### Revert a commit that is already pushed to server (not the last commit)

To skip the editor and use the default message
```sh
git revert <commit-hash> --no-edit
```

Incase you want to give a detailed message for the revert
```sh
git revert <commit-hash>
```

```
```