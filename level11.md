<img width="1125" height="748" alt="image" src="https://github.com/user-attachments/assets/5ca21041-6b63-4374-b645-7e96859883bd" />
So sánh giá trị chẵn/lẻ dùng xor, or, and, không xài mov

<img width="332" height="352" alt="image" src="https://github.com/user-attachments/assets/0b801499-f435-4c77-ae22-d21cc055771a" />
xor rax, rax => rax = 0
or rax, rdi
Lúc này 2 trường hợp
rdi = 1 => rax = 1
and rax, 1 = > 1
xor rax, 1 => 0
->> số lẻ

rdi = 0 => rax = 0
and rax, 1 => 0
xor rax, 1 => 1
->> số chẵn

![Uploading image.png…]()
