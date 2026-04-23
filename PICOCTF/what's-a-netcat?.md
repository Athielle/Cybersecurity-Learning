#PICOCTF: what's a netcat?

Date: 24/04/2026
Goal: Use netcat to connect the given hostname to the given port number.

What I did:
1. I'm clueless about netcat so I used the hint, which only says `nc tutorial`
2. I tried running `netcat man`, nothing useful, only to realize nc tutorial meant netcat tutorial.
3. Searched the internet for netcat tutorial and found an article about netcat commands at `www.varonis.com/blog/netcat-commands`
4. Found `nc -help` and it gave me a summary of netcat commands.
5. Still clueless at this point, so i identified what I have: a hostname/link, and a port number.
6. Seemed similar to the ssh I did before so I tried running `netcat [hostname] -p[port number]`, didn't work. Tried `netcat [hostname] -p [port number]`, still didn't work.
   Tried without the -p, and got the flag. <img width="877" height="359" alt="image" src="https://github.com/user-attachments/assets/e4c6bdb4-6b90-4374-af8e-5aa43ce1b68f" />
7. I didn't understand why, so I searched the internet on how to view a netcat manual page. Turns out its supposed to be `man nc`.
8. In synopsis, I believe I found the syntax which is `nc [destination] [port]` but I did `netcat [destination] [port]` which works just fine. (I tried doing both and got the flag for both). This syntax works because
   I believe the goal is to connect the hostname(destination) to the port number. 

Takeaway:
- Netcat or nc is a networking tool that uses TCP and UDP connections to read and write in a network.
- netcat functions as a utility tool for port scanning and port listening. Some hackers may use it as a back-door
- netcat -help or netcat -h shows a summary of possible commands to use
- man nc is the manual page.
- Most tool manuals follow the syntax `man [toolname]`
- remember that NETCAT AND SSH ARE DIFFERENT, AND THEREFORE WILL HAVE DIFFERENT COMMANDS
