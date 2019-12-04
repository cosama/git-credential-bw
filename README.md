# Git credential helper for bitwarden password manager

Get your git repository username and password automatically from bitwarden, so that you truly only need to know the master password when coding.

## Requirements

Download the bitwarden cli: https://github.com/bitwarden/cli

## Installation

1) Place the git-credential-bw in your system path (for example in `~/.local/bin`)
2) Open a terminal and enter `git config --global credential.helper bw`

## Information

The script is configured now to use `git-credential-cache` (https://git-scm.com/docs/git-credential-cache) to store logging information for later use. This mean the session key for `bw` doesn't need to be shared between instances and your vault is safe at all times. The login information however are available in plain text through `git-credential-cache` and thus this  script (as `git-credential-cache` in general) should only be used on systems where you trust all people with access.
