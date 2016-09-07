# parseable-dash-dash-help

This repository exists to standardize a variant of `--help` output for
command-line programs, which:

1. Is machine parseable
2. Unambiguously specifies the command's grammar

The intention is for such output to be used by the shell's tab completion logic,
by static analyzers of shell scripts, and so on.

We envision that a package manager would install
a `/usr/share/rsync/rsync.grammar` file alongside the `/usr/bin/rsync` binary,
and shells would parse that file instead of hardcoding the list of options
`rsync` takes in their completion functions (such as
[`/usr/share/bash-completion/completions/rsync`][bash:rsync] or
[`/usr/share/zsh/functions/Completion/Unix/_rsync`][zsh:_rsync]).


[zsh:_rsync]: https://github.com/zsh-users/zsh/blob/master/Completion/Unix/Command/_rsync
[bash:rsync]: https://github.com/scop/bash-completion/blob/master/completions/rsync
