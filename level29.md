<img width="1119" height="718" alt="image" src="https://github.com/user-attachments/assets/05e4fb9d-73e0-40dc-b48e-6d73cbef42f2" />
Req: đổi chữ hoa thành chữ thường và trả về số byte của chữ thường

<img width="602" height="664" alt="image" src="https://github.com/user-attachments/assets/16a5f7ea-d863-4a52-b561-a950eed11367" />
<img width="511" height="593" alt="image" src="https://github.com/user-attachments/assets/fd7d75d6-ad59-4f71-93da-1e0116067e23" />

push để trả lại giá trị ban đầu trước khi ret kết thúc hàm
push thêm r13 để stack aligment 16 bytes

đặt i = r12 = 0
mov rbx để giữ lại nguyên địa chỉ rdi trước khi ret kết thúc hàm

compare địa chỉ = 0 thì ret 0

loop_start:
byte = 0 thì ret 0
check nếu là chữ thường thì skip check chữ tiếp theo
còn không thì gán byte tại [rbx] rồi set vào rdi
gọi hàm foo
trả về kết quả 1 bytes là al, sau đó gắn ngược lại [rbx]
r12+ nghĩa là đã có 1 chữ hoa thành chữ thường

skip:
qua chữ tiếp theo
quay lại loop_start để check

done:
trả kết quả về rax
rồi push để trả lại giá trị ban đầu rồi return giá trị rax cho máy

<img width="1222" height="715" alt="image" src="https://github.com/user-attachments/assets/ced0635e-9c8b-4247-a63d-6ca91ed92d47" />
