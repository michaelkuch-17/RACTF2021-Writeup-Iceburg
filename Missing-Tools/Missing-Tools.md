## Known Information
### Disclaimer! Unintended Solution Found - proper solution tbf
##### username: ractf
##### password: 8POlNixzDSThy
##### Given Info on Flag:
##### ![Given Info](https://github.com/michaelkuch-17/RACTF2021-Writeup-Iceburg/blob/main/Missing-Tools/missing-tools-info.PNG)
---
##### First step was to ssh into the shell and find the usable commands.
```
ssh ractf@193.57.159.27 -p(given port)
```
##### On password prompt, enter given password
---
##### On entering the shell, many commands are unavailable or are disabled by the administrator. Common commands such as ls, cat, vi, vim, etc. are not usable.
##### Commands that are available are found in when running /opt/toybox.
##### ![Usable commands](https://github.com/michaelkuch-17/RACTF2021-Writeup-Iceburg/blob/main/Missing-Tools/missing-tools-usable-commands.PNG)
##### Within the /home/ractf directory, we are able to find any files/directorys are available.
```
$ echo *
```
##### This shows that flag.txt is stored here. We now have our objective in scope, view the contents of flag.txt to secure the flag!
---
##### From here, a lot of time was spent trying to break out of the terminal. Gaining access to vi, bash, thoughts of bruteforcing the root password, set environment variables, and a lot of other hot garbage.
##### The short answer to this is that the flag was found accidentally. Running, `$ source flag.txt` the flag is given as below.
**Flag: ractf{std0ut_1s_0v3rr4ted_spl1t_sha}**
---
##### While the flag was found and is correct, the method of discovery was most likely not the intended method.
##### The following section will be left blank, in an attempt to find the correct solution or a write-up of the correct solution will be linked.
## Correct solution
