#PICOCTF: Insp3ct0r

Date: 05/05/2026
Goal: Look for the flag hidden in the web code

What I did:
1. this challenge is categorized as a web exploitation, so I was honestly nervous. The moment I ran the instance, it gave me a link but it is not clickable. This is a web exploit so I will not use the webshell or wget.
2. I highlighted the link and right-clicked, then selected the "Go to web address" to access it.
3. Once its running, I checked the hint as this is my first web exploit. It says "How do you inspect web code on a browser?". The word "inspect" gave me the clue.
4. On the website, I right-clicked and hit the "Inspect element", which showed me the skeleton of the website.
5. Hint 2 gave me "There are 3 parts"
6. Went back to the website and looked for anything that is 3 parted. I clicked every clickable element, and on the How tab is a specific 3 line: HTML, CSS, JS (Javascript).
7. I believed thats it, so I looked back at the Inspect elemen ton the side
