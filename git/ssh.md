
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
#### Change local user name and email

```sh
git config --local user.name "my-user-name"
git config --local user.email "github-email"
```

```sh
git commit -S -m "YOUR_COMMIT_MESSAGE"
```