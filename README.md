# wineprc

Manage wine (winehq.org) processes. Bash script.

Why we need this: wine itself doesn't provide a effecient way to manage their processes. Even `wineserver -k` sometimes doesn't work.

## Features

- List wine processes
    - WINEPREFIX
    - PID (Unix)
    - The process status, zombie or not
    - Command
    - Full command 
    - Window(s) Title(s) (some windows or processes can't get, due to some X11 mechanism)
- Kill wine processes
    - Choose SIGINT or SIGKILL
    - Choose a WINEPREFIX to kill, or kill all

## Usage
```
Usage:

    -h, --help              Show this help

    -l, --list              List all running wine processes
    
    -k <WINEPREFIX>         Kill a running WINEPREFIX.
                            Use 'all' to kill all WINEPREFIX
    -kk                     Same as '-k' but kill with SIGKILL
```
