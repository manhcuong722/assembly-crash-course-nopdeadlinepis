Run file

<img width="1212" height="745" alt="image" src="https://github.com/user-attachments/assets/066eb3f0-ecad-4181-9da7-25878417ec65" />

Require:

Move rdi register's value to the rax register, then divide by rsi

<img width="378" height="321" alt="image" src="https://github.com/user-attachments/assets/c24b2b0d-3bc8-41ed-b418-71d6abc1c04a" />

After running the script, we got this

<img width="1274" height="769" alt="image" src="https://github.com/user-attachments/assets/32c5fdd0-750f-4208-a738-0f10859f85d0" />

The reason why I set the rdx register's value to 0 is because div doesn't just divide rax only, it divide both rax and rdx together as a single 128-bit, so I set the rdx to 0 to make the rax register's value is the only one get divided
