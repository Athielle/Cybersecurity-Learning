#PICOCTF: Mod 26

Date:25/04/2026
Goal: Decipher the given text file.

What I did: 
1. In the description of the challenge, I was asked if I know what ROT13 is. I had a hunch it was gonna be Rotation 13,
   but searched anyway, and it is Rotation 13. I was interested in cryptography before, from detective novels I read.
2. I downloaded the text file provided in the description.
3. I tried doing it how I remembered doing it. It looked wrong if I compared it to previous flags, but I entered it anyway, and yes it was wrong.
4. I searched how to do it, turns out it `replaces a letter with the 13th letter AFTER IT`. So its not a=m, but rather a=n.
5. Got the flag.
6. <img width="2440" height="1712" alt="Rot13" src="https://github.com/user-attachments/assets/6915ee59-fb8b-454d-9cc0-3e1b69e49c78" />


Takeaway:
- ROT13 or rotation 13 is a substitution cipher that replaces a letter with the 13th letter AFTER it.
- It's not the most secure cipher, its fun but not secure.
- If ROT13 is used twice on the same set of letters, it'll revert back to its plaintext form since the alphabet has 26 letters.
