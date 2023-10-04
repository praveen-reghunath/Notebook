
### Create ssh key
```
ssh-keygen -t ed25519 -C "praxxx.xxxxx@gmail.com"
```

### Copy ssh key to clipboard
```
pbcopy < ~/.ssh/id_ed25519.pub  
```

### See all git config
```
git config --list
```

### See a specific item
```
git config user.name
git config user.email
```

### Config an item

```
 git config --global user.email "praxxx.xxxxx@gmail.com"
```
