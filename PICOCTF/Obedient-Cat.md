#PICOCTF: Obedient Cat

Date: 21/04/2026
Goal: Find the flag

What I did:
The challenge provided a link named 'flag' after the description "This file has a flag in plain sight (a.k.a in-the-clear)". Having started it without any preparation, I used hints. The hint showed the command
`wget` and the link to the flag. 
1. I opened the web-based terminal shell.
2. I typed in `wget [link]`.
3. I need to see whats inside the downlaoded file, so I used `cat`, typing in `cat flag`.
4. After that, the contents of the file is shown, and it is the flag to complete the challenge.
   
Takeaway:
- `wget` is a Linux command that lets me download files from the internet through the command line
- `cat` short for concatenate, helps me view the contents of a file instantly.
