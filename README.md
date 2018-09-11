# gcp-tools
Tools for Google Cloud Platform

## Installation

Install scripts in bin/ in anywhere under $PATH.

### Requirement

Install [gcloud](https://cloud.google.com/sdk/gcloud/)
and set an account.

### Usage

#### Google Compute Engine Management

    $ gce list              # Show compute instance list
    $ gce ls                # Same as list
    $ gce start  [instance] # Start insatnce
    $ gce stop   [instance] # Stop insatnce
    $ gce delete [instance] # Delete instance
    $ gce rm     [instance] # Same as delete
    $ gce ssh    [instance] # SSH to instance
    $ gce create [instance options...] # Create instance
    $ gce make_image <input instance name> <output image name> # Make image from the instance

For start, stop, delete(rm), and ssh,
if `instance` is not given, then a selection mode starts and 
you can select an instance on which the command is executed.

For start, stop, delete (rm), multiple instances can be selected.

### Option

Tools will use following tools for the selection if installed:

- [peco](https://github.com/peco/peco)
- [fzy](https://github.com/jhawthorn/fzy)
- [fzf](https://github.com/junegunn/fzf)
- [sentaku](https://github.com/rcmdnk/sentaku/)

if they are installed.

Otherwise shell's `select` is used.

