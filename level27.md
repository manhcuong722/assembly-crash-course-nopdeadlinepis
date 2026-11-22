<img width="999" height="842" alt="image" src="https://github.com/user-attachments/assets/a8d905be-5531-420b-8f05-4498447569d3" />

Req: vòng lặp tính tổng rồi chia trung bình

<img width="423" height="506" alt="image" src="https://github.com/user-attachments/assets/2ff54950-ee5d-43df-bd0d-07c1b189a3a6" />

rdi: địa chỉ gốc
rax: kết quả
rsi: n
rcx: i

xor rax, rax với xor rcx, rcx để 2 cái = 0 

loop_start
compare rcx với rsi ( i với n )
nếu i >= n => loop end

còn không thì sum add giá trị tại địa chỉ [rdi + i*8 bytes]

xong thì loop end
set rdx = 0 để khi chia thì chỉ chia của rax chứ không phải cả rax và rdx

<img width="1108" height="616" alt="image" src="https://github.com/user-attachments/assets/ca37e8b1-97c4-4d71-9ce3-61adffd6c5cd" />

