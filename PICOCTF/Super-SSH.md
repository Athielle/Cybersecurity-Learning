#PICOCTF: Super SSH

Date:23/04/2026
Goal: Find the flag

What I did:
1. I ran the Instance in which it gave me the whole description of the challenge.
2. I opened the webshell and realized I don't know what to do.
3. I opened the link `https://linux.die.net/man/1/ssh` and learned the ssh format.
4. I identified the username, host, and the port from the description.
5. I typed `ssh username@host -p [port number]`.
6. I followed the rest of the instruction given in the description and finished the challenge.

Takeaway:
- the format to ssh is `ssh username@host...`, then depends on what you wanna do with ssh, there could be
  different commands
- `-p` is for the port to connect to on the remote host. 
- ssh, by default, uses port 22, so using `-p` will help specify the target port
- Casing of the letters is important as upper case letters have different purpose than lower case letters.
- Spaces in between of the commands (`-p [port number]`] might also affect the syntax.
