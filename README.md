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
 Tên Bài:  Hai kiểu kết nối ở Tầng Transport. So sánh hai kiểu kết nối đó. Đặc điểm của các giao thức tương ứng với từng kiểu kết nối.  
 ----  
 ### 1. Hai kiểu kết nối ở Tầng Transport. So sánh hai kiểu kết nối đó. Đặc điểm của các giao thức tương ứng với từng kiểu kết nối.  
  - Việc truyền thông điệp trực tiếp hay kết nối các ứng dụng tại tầng giao vận có thể được phân loại như sau:
          - **định hướng kết nối (connection-oriented)**,*ví dụ TCP*  
              - Định hướng kết nối (Connection-oriented) là cách truyền thông cần kết nối 2 thiết bị gửi và nhận trước khi truyền dữ liệu, phương pháp này gọi là dịch vụ mạng đáng tin cậy. Nó đảm bảo dữ liệu sẽ chuyển đến đúng nơi yêu cầu, các dịch vụ hướng kết nối thiết lập các liên kết ảo giữa hai hệ thống gửi và nhận thông qua mạng. 
              - **TCP(Tranmission Control Protocol):** là giao thức truyền tải connection-oriented điển hình .  
              - *Một giao thức connection-oriented (hướng kết nối) mang các đặc điểm như sau:*  
                  - Phải thực hiện thiết lập kết nối với đầu xa trước khi thực hiện truyền dữ liệu. Tiến trình thiết lập kết nối ở TCP được gọi là tiến trình bắt tay 3 bước (threeway handshake).  
                  - Phải thực hiện cơ chế báo nhận khi truyền dữ liệu. Mọi segment được gửi đi đều phải được báo nhận (acknowledge, hay viết gọn là ack). Các segment gửi đi mà không được báo nhận xem như bị lỗi khi truyền và sẽ được thực hiện truyền lại.   
                  - Phải thực hiện cơ chế đánh số thứ tự (sequencing) cho các đơn vị dữ liệu được truyền.  
                  - Phải thực hiện các cơ chế điều khiển luồng thích hợp (flow control) để tránh nghẽn xảy ra.  
          ![img](https://www.adminvietnam.org/wp-content/uploads/2016/10/tcp-segment.png)  
        - **phi kết nối (connectionless)**, *ví dụ UDP*  
                  - UDP (User Datagram Protocol) là một giao thức truyền tải connectionless điển hình. Một giao thức connectionless sẽ không thực hiện thao tác xây dựng kết nối trước khi truyền dữ liệu mà thực hiện truyền ngay lập tức khi có dữ liệu cần truyền (gọi là kiểu truyền best effort – truyền tổng lực). Ngoài ra phương thức truyền connectionless cũng không sử dụng các phương pháp đảm bảo độ tin cậy như báo cáo nhận hay điều khiển luồng (flow control). Connectionless không thực hiện các biện pháp đánh số thứ tự cho các đơn vị dữ liệu được truyền…  
       ![img](https://www.adminvietnam.org/wp-content/uploads/2016/10/udp-datagram.png)  
         
----  
Tên Bài: Quy trình bắt tay 3 bước (three way - handshake) trong tầng Transport  
----  
 ### 1.Quy trình bắt tay 3 bước (three way - handshake) trong tầng Transport?  
  - **TCP thiết lập kết nối bằng 3 bước bắt tay (3-way handshake)**
  ![img](https://www.adminvietnam.org/wp-content/uploads/2016/10/3-buoc-832x420.png)

|sender              |  receiver                     |
|--------------------|-------------------------------|
|SYN seq=X---------->|SYN received (step 1)          |
|SYN received<-------|send ACK X+1 and SYN Y (step 2)|
|Send ACK Y+1------->| (step 3)                      |  



  

