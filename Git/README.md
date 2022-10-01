# Git

## Useful commands
[ohshitgit](https://ohshitgit.com/)

## Better difftool under Linux
[Meld](https://meldmerge.org/)

## Only type passphrase once per terminal session
1. `eval "$(ssh-agent -s)`
2. `ssh-add ~/<path>/id_rsa`
3. Add previous command to `~./bashrc`

[Source](https://linuxkamarada.com/en/2019/07/14/using-git-with-ssh-keys/)

## Git branch in terminal
Add to end of `~/.bashrc`:
```
parse_git_branch() {
git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/ (.)/ (\1)/'
}
export PS1="[\033[01;34m]\u@\h [\033[32m]\w[\033[33m]\$(parse_git_branch)[\033[00m] \n$ "
```
