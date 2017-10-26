Người Thực Hiện: Trần Thị Ngọc    
Ngày Cập Nhật: 26/10/2017  
-----  
Tên Bài: Chức năng của tầng Transport  
-----  
### 1.Tầng Transport là gì?  
*Tầng 4: Tầng vận chuyển (Transport Layer)*  
  - Đảm bảo truyền tải dữ liệu giữa các quá trình. Dữ liệu gởi đi được đảm bảo không có lỗi, theo đúng trình tự, không bị mất mát, trùng lắp. Đối với các gói tin có kích thước lớn, tầng này sẽ phân chia chúng thành các phần nhỏ trước khi gởi đi, cũng như tập hợp lại chúng khi nhận được.  
### 2.Nhiệm vụ của tầng Transport?  
  - **Tầng giao vận chịu trách nhiệm truyền phát đầu cuối end – to – end của toàn bộ thông điệp ( trong khi tầng mạng quan tâm tới việc truyền phát đầu cuối của từng gói tin). Tầng giao vận đảm bảo rằng toàn bộ thông điệp truyền đi là toàn vẹn và đúng thứ tự. Ngoài ra chúng cũng xem xét kiểm soát lỗi , kiểm soát luồng dữ liệu ở cấp độ nguồn – đích.** 
 ----  
 Tên Bài: 
 ----  
 Tên Bài: Quy trình bắt tay 3 bước (three way - handshake) trong tầng Transport  
 ----  
 ### 1.Quy trình bắt tay 3 bước (three way - handshake) trong tầng Transport?  
  -**TCP thiết lập kết nối bằng 3 bước bắt tay (3-way handshake)**

|sender              |  receiver                     |
|--------------------|-------------------------------|
|SYN seq=X---------->|SYN received (step 1)          |
|SYN received<-------|send ACK X+1 and SYN Y (step 2)|
|Send ACK Y+1------->| (step 3)                      |  



  

