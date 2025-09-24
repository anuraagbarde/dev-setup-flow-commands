# multi-github-ssh
vim ~/.ssh/config
```config
Host github.com
  AddKeysToAgent yes
  IdentityFile ~/.ssh/exponent-mac-pro-github

Host personalgithub.com
  HostName github.com
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/anuraagbarde@gmail.com_github_rsa
```

```bash
ssh-add ~/.ssh/anuraagbarde@gmail.com_github_rsa

ls 
anuraagbarde@gmail.com_github_rsa     exponent-mac-pro-github
anuraagbarde@gmail.com_github_rsa.pub exponent-mac-pro-github.pub
known_hosts config


ssh-add -l
ssh-add ~/.ssh/anuraagbarde@gmail.com_github_rsa
ssh -T git@personalgithub.com
```
