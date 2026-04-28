#PICOCTF: 2warm

Date: 28/04/2026
Goal: Convert the decimal value into binary value.

What I did:
1. I remembered how to convert from my uni days. In fact, I believe it is one of my favorite
   topics back then. I believe it was when we were learning IP addresses and subnetting. So
   wrote down the place values: `128 64 32 16 8 4 2 1`, 8 bits. 
2. I wrote a `1` on the values `32 8 2` and added them together to get the value of `42`.
3. I got `00101010`. I tried answering this and the flag said it was incorrect.
4. I removed the first two zeroes, so it was just `101010`, and got it right this time.
   <img width="2980" height="1908" alt="2warm" src="https://github.com/user-attachments/assets/e84df276-9f92-451c-9598-3befd1c99c82" />

Takeaways:
- The zeroes at the front will be ommitted as it works as a place value.
- In Subnetting however, I believe I need to include the zeroes to shows the full octet.
