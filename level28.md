<img width="1012" height="863" alt="image" src="https://github.com/user-attachments/assets/9706ef0d-a10f-4c44-958f-39acc4f0c468" />

Req: đếm xem có bao nhiêu số liên tiếp khác 0 

<img width="521" height="486" alt="image" src="https://github.com/user-attachments/assets/efc3e077-288a-4ff1-8012-33d0b8f02ef5" />

đặt rax = 0
so sánh byte tại rdi, nếu = 0 thì end

không thì loop_start
so sánh giá trị bytes mà địa chỉ [rdi + rax] trỏ tới, nếu = thì jump done
không thì rax +1 rồi quay lại loop

<img width="1175" height="735" alt="image" src="https://github.com/user-attachments/assets/fc3f7ac1-be04-42ac-951f-bb7fdc2acf0d" />
