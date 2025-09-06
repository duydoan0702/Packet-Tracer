<img width="784" height="516" alt="image" src="https://github.com/user-attachments/assets/04639e3f-2eb3-46a7-bc55-402abb10d879" />

# YÊU CẦU
1. Máy A ping được tới máy B,  máy A ping được tới máy C
2. Máy B ping được máy C

# THỰC HIỆN
? A ping được B, A ping được C
- Ta cấu hình cho A chung mạng với B `192.168.1.2`, tương tự với A và C `192.168.2.2`. Ta cấu hình 2 card mạng cho máy A với 2 địa chỉ mạng `192.168.1.1` và `192.168.2.1`

? B ping được C
- Thêm router vào để định tuyến giữa `192.168.1.0/24` và `192.168.2.0/24`. Ta cần cấu hình thêm `default gateway` để giao tiếp với máy bên mạng khác. Nếu không có chỉ có thể giao tiếp trong cùng `subnet mask`.

# KIẾN THỨC
- **Default gateway** là địa chỉ IP của cổng router nằm trong cùn mạng với PC, PC sẽ gửi gói tin ra ngoài mạng thông qua địa chỉ này.
