#PICOCTF: Insp3ct0r

Date: 05/05/2026
Goal: Look for the flag hidden in the web code

What I did:
1. this challenge is categorized as a web exploitation, so I was honestly nervous. The moment I ran the instance, it gave me a link but it is not clickable. This is a web exploit so I will not use the webshell or wget.<img width="940" height="685" alt="image" src="https://github.com/user-attachments/assets/0a68e9f0-671e-47a0-974d-9c3f628fe8e4" />

2. I highlighted the link and right-clicked, then selected the `Go to web address` to access it.
3. Once its running, I checked the hint as this is my first web exploit. It says "How do you inspect web code on a browser?". The word "inspect" gave me the clue.
4. On the website, I right-clicked and hit the `Inspect element`, which showed me the skeleton of the website.
5. Hint 2 gave me "There are 3 parts"
6. Went back to the website and looked for anything that is 3 parted. I clicked every clickable element, and on the How tab is a specific 3 line: HTML, CSS, JS (Javascript).
7. I believed thats it, so I looked back at the Inspect element on the side. The html is easy enough as it is the first to show.
8. I checked every line and saw a comment where the first of the three of the flag is.
9. The CSS abd Javascript though, as I am no longer familiar with the layout, I had to check every tab. I landed on the Source tab where there are 3 files namely: (index), myjs.js, and mycss.css, where I found the rest of the flag.
<img width="940" height="891" alt="image" src="https://github.com/user-attachments/assets/1355ea47-0b75-461b-bb30-0eb8a598ee1c" />
<img width="940" height="887" alt="image" src="https://github.com/user-attachments/assets/50cd7c00-e32b-41e1-959a-ea1800855038" />
<img width="940" height="650" alt="image" src="https://github.com/user-attachments/assets/66ab8041-cc53-4c57-a7ee-90355606141c" />

Takeaway:
- The `Inspect element` is one of the tool used in web exploitation. It allows the user to see how their browser is structured.
- Comments are invisible in the webpage itself, but anyone accessing the inspect element will be able to see it. Comments with sensitive information will also be seen, so its best not to include any personal or sensitive information.
- From my stock knowledge of web development, HTML, CSS, and Javascript is the building blocks of every webpage. HTML is the skeleton, the structure of how the website is built. CSS is for styling as it stands for Cascading Style Sheet. It involves fonts, and other elements that is present in the actual web page. Javascript is how its gonna behave.
- The `Source` tab is where the files for html, css, and javascript are located. 
