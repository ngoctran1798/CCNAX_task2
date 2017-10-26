Người Thực Hiện: Trần Thị Ngọc    
Ngày Cập Nhật: 26/10/2017  
-----  
Tên: Chức năng của tầng Transport  
-----  
### 1.Tầng Transport là gì?  
**Tầng 4: Tầng vận chuyển (Transport Layer)**  
  - Đảm bảo truyền tải dữ liệu giữa các quá trình. Dữ liệu gởi đi được đảm bảo không có lỗi, theo đúng trình tự, không bị mất mát, trùng lắp. Đối với các gói tin có kích thước lớn, tầng này sẽ phân chia chúng thành các phần nhỏ trước khi gởi đi, cũng như tập hợp lại chúng khi nhận được.  
### 2.Nhiệm vụ của tầng Transport?  
  - Transport làm nhiệm vụ vận chuyển thông tin từ nguồn tới đích. Tầng Transport nhận dữ liệu nhận từ tầng Application rồi đóng gói bằng giao thức TCP hoặc UDP để vận chuyển đi.  
  - Cho phép truyền đồng thời nhiều bản tin của các dịch vụ khác nhau trên cùng một đường truyền.  
      - Transport sử dụng cơ chế phân đoạn dữ liệu (Segmentation), cơ chế quản lý truyền dẫn và nhận diện dịch vụ bằng port nên có thể truyền bản tin của các dịch vụ khác nhau trên cùng một đường truyền, tiết kiệm băng thông đường truyền, dễ truyền và sửa lỗi. Đồng thời khi truyền dữ liệu từ nguồn tới đích sẽ có kích thước khác nhau. Để dữ liệu chuẩn theo kích thước truyền thì sẽ phân đoạn thành nhiều đoạn.  
      - Máy nguồn gửi dữ liệu sử dụng cơ chế phân đoạn thì bên máy đích sẽ nhận dữ liệu theo đúng trật tự ban đầu.  
  - Hỗ trợ truyền thông tin cậy khi được yêu cầu: sử dụng cơ chế bắt tay 3 bước để xác nhận thông tin.  
  - Cho phép quản lý lỗi: thông qua giao thức TCP nó sẽ truy vết quá trình truyền thông từ nguồn tới đích. Đồng thời khi có lỗi xẩy ra nó sẽ yêu cầu truyền thông lại các segment bị lỗi.  
  - Nhận diện các dịch vụ khác nhau: khi cho phép truyền nhiều ứng dụng sẽ gán port đích cho mỗi dịch vụ để biết đâu là DNS, Web, EMail…  
  







