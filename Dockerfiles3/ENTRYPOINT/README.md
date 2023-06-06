### ENTRYPOINT
Entrypoint is used to run the container same as CMD, but there are few differences. 

Entrypoint can't be overriden but we can override CMD.

#ping -c5 google.com ping c2 apple.com -- if we override entrypoint with a command, that command is appended to the first command.

for best practices we use CMD and ENTRYPOINT in combination.

If we use both CMD and ENTRYPOINT, and we don't enter the argument in terminal, then CMD acts as a argument provider to the ENTRYPOINT.

CMD will  provide default arguments to the ENTRYPOINT.

You can alwalys override CMD rguments from rumtime.