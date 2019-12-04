# Git credential helper for bitwarden password manager

Get your git repository username and password automatically from bitwarden, so that you truly only need to know they master password when coding.

## Requirements

Download the bitwarden cli: https://github.com/bitwarden/cli

## Installation

1) Place the git-credential-bw in your system path (for example in `~/.local/bin`)
2) Open a terminal and enter `git config --global credential.helper bw`
