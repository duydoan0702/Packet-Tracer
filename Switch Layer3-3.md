<img width="1186" height="557" alt="image" src="https://github.com/user-attachments/assets/1c0951b0-ae9c-4db9-b6d0-9a18db7b676e" />

# Yêu Cầu
- A ping qua B, Gói tin request đi qua C và gói tin reply đi về qua D

# Cách làm

1. Ta thiết lập IP và chuyển switch layer 3 thành router và đặt lại các địa chỉ cho switchport như trên ảnh.
2. Ta muốn đầu tiên gói request đi lên switchC nên ta phải đặt `default gateway` trỏ đến địa chi routeip của SwitchC
3. Tương tự ta muốn gói reply đi xuống SwitchD ta phải đặt `default gateay` trỏ đên sđịa chỉ routeip của SwitchD
