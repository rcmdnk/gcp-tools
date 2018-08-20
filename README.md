# gcp-tools
Tools for Google Cloud Platform

## Installation

Install scripts in bin/ in anywhere under $PATH.

### Requirement

Install [gcloud](https://cloud.google.com/sdk/gcloud/)
and set an account.

### Option

Tools will use following tools for the selection if installed:

- [peco](https://github.com/peco/peco)
- [fzy](https://github.com/jhawthorn/fzy)
- [fzf](https://github.com/junegunn/fzf)
- [sentaku](https://github.com/rcmdnk/sentaku/)

if they are installed.

Otherwise shell's `select` is used.

