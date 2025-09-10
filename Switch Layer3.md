<img width="723" height="445" alt="image" src="https://github.com/user-attachments/assets/d324ca22-1da3-4eab-be74-da2b0af96845" />

# YÊU CẦU
- Ping 2 máy khác mạng A qua B.
# Thực Hiện
- Vì 2 máy khác mạng nên phải có router để có `default gateway` để đi sang mạng khác. Nên ta chuyển Switch Layer 3 thành `router` bằng câu lệnh.

```
ip routing
```
- Bình thường, các cổng FastEthernet/GigabitEthernet trên switch đề là switchport và hoạt động ở layer2. Nên ta cần chuyển sang chế độ `Layer routed port` làm cổng trở thành cổng như trên router và có thể gán IP.

```
interface fa0/1
no switchport
ip address 192.168.1.1 255.255.255.0
no shutdown
```

- Ở bước cuối ta chỉ cần thiết lập `default gateway` nữa là xong.
