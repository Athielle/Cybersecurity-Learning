#PICOCTF: Bases

Date: 29/04/2026
Goal: Find the meaning of the given base64

What I did:
1. I have no idea how to do this challenge and the hint only says how to submit the answer. Based on the name of the challenge, I know its gonna be a base but I still have no idea how to do it.
2. I ended up searching the specific challenge and saw a blogpost from someone (`https://medium.com/@walterchristian28/picoctf-2019-bases-1f224af8c9cc`) who tackled the challenge, so I can't take credit for this challenge's completion.
3. I still tried to do the procedure, and compare my answer to theirs. Mine was wrong because of a single letter I mistyped, but I got the flag when I corrected it.
   <img width="392" height="45" alt="image" src="https://github.com/user-attachments/assets/ed4d4acf-e82a-4e09-b165-112ef23c7aed" />


Takeaway:
- The challenge uses base 64, a way of encoding binary data into a format that only uses text characters. It embeds data in text format, meaning it allows the inclusion
  of binary data within text-based files, which is useful for displaying images in webpages or sending attachements in emails.
- It offers the obfuscation or the process of obscuring the intended meaning of a data, though it is not a strong encryption so it must not be heavily relied on.
- base64 decoding can be done on the terminal in three ways (at least that's how many I read from the tutorial I searched for this challenge.)
  > Decoding the string by copying it and pasting it in the terminal as such `base64 -d "string"`
     I tried this on my terminal and it returns the "No such file or directory." I may have misunderstood this one.
  > Decoding the string by converting it to a file, `base64 -d "string" > decodedtext.txt`
     I tried doing it how it was shown, but it didn't do anything. Then I used the format from the third method and mix it with what is said here which game me
     `echo "bDNhcm5fdGgzX3IwcDM1" | base64 -d > file.txt`, then I forgot the command `cat` before calling the file so it gave me "-bash: file.txt: command not found".
     I then used `cat file.txt`, and got the flag.
  <img width="571" height="151" alt="image" src="https://github.com/user-attachments/assets/7772bf28-1c8e-4e61-9376-83c030c16e38" />
  > By directly using echo and base64 command, `echo "string" | base64 -d`
     I did this one simply because it looks to be the easiest.
- `|` this is called a pipe. It takes the value on the left and gives it to the right, is how i understand it.
