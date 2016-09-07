# parseable-dash-dash-help

This repository exists to standardize a variant of `--help` output for
command-line programs, which:

1. Is machine parseable
2. Unambiguously specifies the command's grammar

The intention is for such output to be used by the shell's tab completion logic,
by static analyzers of shell scripts, and so on.
