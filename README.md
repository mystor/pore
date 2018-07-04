# pore - A Pretty Okay Remote Environment

pore is a tool for remote software development. It is intended to enable
local editing and version control, while using a remote machine for builds.
Pores are associated with git repositories, using *git config* for configs.

## Install

To install pore, add the `pore` executable to your path.

Pore depends on some external programs which must also be installed and on your path:
1. [`lsyncd` 2.2.3+](https://github.com/axkibe/lsyncd)
2. [`python` 3.6+](https://www.python.org/)
3. [`git`](https://git-scm.com/)
4. `ssh`, `sh`, and `flock` (which are probably already installed)

## Usage
```
pore [options]
options:
   -i, --inject [<cmd>...]  run <cmd> on the remote
   -o, --open               open pore, if needed
   --close                  close pore and exit
   --dump=<what>            print pore status / config info and exit
   --help                   show a detailed help message
```

Detailed usage information is included in the module documentation, which can
be viewed with the '--help' command line option
