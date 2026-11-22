<img width="1040" height="473" alt="image" src="https://github.com/user-attachments/assets/dc2221c4-e1a0-4ca7-86e4-a8676583c9c0" />

Req: xài if + compare để so sánh, ở đây xài thanh ghi eax và ebx vì dữ liệu liền kề nhau cách 4 bytes

<img width="409" height="700" alt="image" src="https://github.com/user-attachments/assets/89e79107-4e7c-4650-b9dc-a8d26923d151" />

gán giá trị tại địa chỉ rdi vào ebx
compare => ko bằng nhảy tới check2
không thì add thêm 3 giá trị liền kề rồi nhảy tới done

ở check2, compare ko bằng => nhảy tới other nhân 3 giá trị liền kề nhau 4 bytes rồi tới done
còn bằng thì tiếp tục => trừ hết rồi nhảy tới done

<img width="1157" height="735" alt="image" src="https://github.com/user-attachments/assets/1d6aabd7-2bd2-401b-984b-f59e0b780359" />
