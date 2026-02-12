
### Create ssh key
```sh
ssh-keygen -t ed25519 -C "praxxx.xxxxx@gmail.com"
```

### Copy ssh key to clipboard
```sh
pbcopy < ~/.ssh/id_ed25519.pub  
```

### See all git config
```sh
git config --list
```

### See a specific item
```sh
git config user.name
git config user.email
```

### Config an item

```sh
 git config --global user.email "praxxx.xxxxx@gmail.com"
```
#### Change user name and email for a specific repo

```sh
git config --local user.name "my-user-name-not-the-display-name"
git config --local user.email "the-github-email-copy-from-github-settings"
```
