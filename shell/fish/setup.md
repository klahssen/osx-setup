# Fish shell

## install the shell
download the installer from https://fishshell.com

## oh-my-fish
for customization
https://github.com/oh-my-fish/oh-my-fish

- install
`curl -L https://get.oh-my.fish | fish`

- install a theme
`omf install bobthefish`

- fish config file default location is ~/.config/fish
- put the content of this directory in ~/.config/fish

- setup the fish prompt
set -g theme_display_git_master_branch yes
set -g theme_display_git_dirty yes
set -g theme_display_k8s_context yes
set -g theme_git_worktree_support yes
set -g theme_git_worktree_support no
set -g theme_display_user ssh
set -g theme_display_hostname ssh
set -g theme_display_cmd_duration yes
set -g theme_powerline_fonts no
set -g theme_show_exit_status yes
set -g theme_color_scheme dark
set -g theme_newline_cursor yes 