
# config
```sh
  git config --global user.email “hello@brightonzhang.com”
  git config --global user.name “Brighton Zhang”
```

# ssh
```sh
ssh-keygen -t rsa -b 4096 -C “argzha@gmail.com”
eval "$(ssh-agent -s)"
ssh-add .ssh/github
cat .ssh/github.pub 
```

# remote

## add remote
```sh
git remote add origin https://github.com/brightonzhang/mommychoose-node.git

git push -u origin master
```

## Switching remote URLs from HTTPS to SSH
```sh
# List your existing remotes in order to get the name of the remote you want to change.
git remote -v
# origin  https://github.com/USERNAME/REPOSITORY.git (fetch)
# origin  https://github.com/USERNAME/REPOSITORY.git (push) 

# Change your remote's URL from HTTPS to SSH with the git remote set-url command.
git remote set-url origin git@github.com:USERNAME/REPOSITORY.git

# Verify that the remote URL has changed.
git remote -v
# Verify new remote URL
# origin  git@github.com:USERNAME/REPOSITORY.git (fetch)
# origin  git@github.com:USERNAME/REPOSITORY.git (push)
```