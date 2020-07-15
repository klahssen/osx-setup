# SETUP 

## go get needs force git to ssh
edit the config file
`git config --global --edit`

then add replacement for the targets

example:
[url "ssh://git@gitlab.com/"]
  insteadOf = https://gitlab.com/



## ref .gitconfig
put the reference .gitconfig in ~/.gitconfig if you don't
want to manually edit it.
