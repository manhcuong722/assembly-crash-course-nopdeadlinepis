LEVEL 1 TRONG ASSEMBLY CRASH COURSE

First of all, I ran the file that the challenge gave me by using the commands /challenge/run

<img width="1216" height="238" alt="11111" src="https://github.com/user-attachments/assets/967d8397-cec1-4c0b-8b01-f3f99e71a006" />

In this challenge, we see that the challenge requires us to change the value of the rdi register to 0x1337

So I wrote a script using Pwntools in Python

<img width="379" height="356" alt="image" src="https://github.com/user-attachments/assets/db9cd834-4edf-46e4-8d95-5cef07ff6538" />

I used context.arch to tell Pwntools which architecture to assemble for
code = asm("rdi, 0x1337") to convert assembly code into machine code 
