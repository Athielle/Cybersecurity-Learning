#PICOCTF: Warmed Up

Date: 27/04/2026
Goal: Convert hexadecimal into a decimal.

What I did:
1. I kind of have stock knowledge from when I was in uni on how to convert, but I've forgotten most of it.
2. The given hexadecimal is 0X3D. I know that after 9, the values of 10-15 is A-F. What I'm confused is the start: 0X.
3. I first worked on the 3 and D. 3 = 3 and D = 13. 3x16^1 + 13x16^0 = n. 3x16 + 13x1 = n. 48+13 = n. 61.
4. But I'm wondering what the 0X is for. After searching and landing into `https://www.freecodecamp.org/news/hexadecimal-number-system/`,
   I learned that 0X is a prefix used to identify a hexadecimal.
5. So the final answer would be 61. <img width="2560" height="1640" alt="hexadecimal" src="https://github.com/user-attachments/assets/615cd4e9-e58d-4165-981b-d34387557285" />

Takeaways:
- Learned that the prefix `0X` is used to indicate a hexadecimal (base 16) and to differentiate it from decimal or octal.
- I confirmed that A through F is valued 10 through 15.
- I need to visit the topic in more depth.
