#PICOCTF: Wave a flag

Date:01/05/2026
Goal: Get the flag

What I did: 
1. I thought it was gonna be similar to my first picoctf challenge, obedient cat, but this comes with a little bit extra steps.
2. I clicked on hint 2, and as expected the `wget`command is needed. The file is downloaded.
3. Hint 3 told me to use the `chmod +x` command with the file name to make it executable. I'm familiar with this command as I've encountered it before but I can't say I remembered what is was for.
4. I then ran the command `./warm` and the file told me to pass it an -h command.
5. I did, but it returned a `-bash: -h command not found`. I think I needed to include the program?
7. Yes, I needed to. I ran `./warm -h` and it gave me the flag.
8. <img width="864" height="405" alt="image" src="https://github.com/user-attachments/assets/3da0a866-d059-4b81-a8bf-75a77dbb22c8" />

Takeaway:
- I need to analyze and understand the description given.
- `chmod` also "change mode" is a command to change the access permissions of files and directories. (https://www.geeksforgeeks.org/linux-unix/what-does-chmod-x-do-and-how-to-use-it/)
- the operation `+x` stands for `+: add permission` and `x: grant permission`, thus `chmod +x warm` granted the file 'warm' the executable permission. If not, the webshell treats it like a text file.
- the webshell couldnt find the command `-h` because it doesnt work alone. By including the program, I am passing the `-h` to the program.
- The documentation for these commands are lengthy but I'll need to read it. Some websites may offer a simple and short explanation, but will still need to double check its authenticity.
