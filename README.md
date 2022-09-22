# ssh-keys V1.0.0

How I use multiple ssh keys for different users with git and vscode

### Create the ssh-keys and associate them with GitHub

Follow https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

### Edit the `~/.ssh/config` file

```
Host <HOST>
    HostName github.com
    IdentityFile ~/.ssh/<SSH KEY FILE>
```

### Edit the `~/.gitconfig` file

```
[url "git@<HOST>:<USERNAME>"]
	insteadOf = https://github.com/<USERNAME>
```
