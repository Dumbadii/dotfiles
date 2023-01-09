- 1. build connect to github
  gen ssh key [github doc gen sshkey](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
  add ssh key to github
- 2.due to clash VPN blocked port 22, change github connect port to 443.
  .ssh/config
- ```
  Host github.com
  User git
  Hostname ssh.github.com
  PreferredAuthentications publickey
  IdentityFile ~/.ssh/id_ed25519.pubf
  Port 443```
  ```
- 3.set git remote