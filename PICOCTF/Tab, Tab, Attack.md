#PICOCTF: Tab, Tab, Attack

Date: 04/05/2026
Goal: Use tab to complete to get the flag.

What I did:
1. I downloaded the given zip file using wget through the webshell.
2. Once downlaoded, I unzip the file using `unzip [file name]`. It showed all the files it created from unzipping it.
3. From the hint provided, it says that hitting the Tab would help me through the long directory. The hint said it would take me 11 tab hits, but I think I only needed 9. I may or may not have done something wrong.
4. I used `ls` before any `cd (tab)` just to go through every directory. Honestly because I did not know I can just tab away without listing anything.
5. After that, I accessed the file inside the innermost directory and used `./` to access it, as I have learned from the previous challenge. And it gave me the flag needed to complete the challenge.
6. I tried this a couple more times, and ended up having a zip file number 7, and it kept asking me if I want to overwrite the existing ones. Personally, I don't like overwriting it and I want to make it look clean.
7. I removed all previous files as if to turn the webshell into a blank slate using `rm -rf [directory] [zip file]*`.
8. I then did everything from start to finish.
9. <img width="1096" height="1102" alt="image" src="https://github.com/user-attachments/assets/4ba17874-7b48-4c02-a236-0f4b898b0c62" />

Takeaway:
- Tab helps the user to complete their command, given that it is within its scope.
- Unzip through the webshell is easier than most software, considering one knows how webshells or command line works, which I'm still in the process of learning myself.
- `./` helps me access a file as it is their address.
- Removing files make use of the command `rm` which means remove. `-rf` is an option within the rm command. `-r` means recursive delete which deletes directories and all its contents. `-f` is force delete which allows the user to delete files without confirmation. It can be written as `-r -f` or `-rf`.
- I also learned that the command `rm -rf` can be a dangeorus tool since it does its job without asking the user for confirmation.
- the `*` at the end means that everything that matches the file preceding it will be included in the command. Better be careful when using these commands as I might delete something I shouldn't.

Update (05/05/2026)
I remembered the command `cat` and wondered if I could've used it instead of `./`. I later learned that those two have different functions. `./` is used to execute a file as if it is a program, while `cat` shows the contents of a file, likely a text file. 
