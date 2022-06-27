# FrontEnd_Architecture
<strong> Làm bất kể cái gì, trong lĩnh vực nào cũng thế, muốn xây dựng cái gì lớn lao thì phải xây dựng được một kiến trúc để theo kiến trúc này mình dễ dạng xây dựng mà sửa chữa mới được. </br> Nhất là trong javascript code nó hơi sexy mà đi mò chức năng thì rất mất thời gian</strong>

- Ở mức tổng thể thì có kiến trúc tổng thể 9phar của TOGAP.
- Ở múc hệ thống thì có kiến trúc hệ thống.
- Ở mức dev thì có kiến trúc phần mềm bao gồm Backend và Frontend.

Trong Frontend chúng ta cần tạo các component theo nguyên tắc SOLID nhưng việc gộp tất cả chúng tạo thành một page lớn thì lại khác, nó phải cần phải có tính tái sử dụng cao, do đó chúng ta cần một kiến trúc mới để có thể dễ dàng lắp ghép nó thành một page. 

Atomic Design với 5 level (Atoms, Molecules, Organisms, Templates, Pages).

Atomic Design là cách tiếp cận kiểu thiết kế giao diện bằng cách xây dựng nên một hệ thống các components thay vì các trang. Phương pháp này chú trọng đến các đối tượng nhỏ, độc lập, tái sử dụng các thành phần để kết hợp chúng lại tạo thành 1 tổng thể. Điều này cho phép hoàn thành sản phẩm nhanh chóng, giao diện thống nhất và dễ dàng bảo trì.

* Atoms: Là thành phần nhỏ nhất, những block cơ bản nhất và không thể nhỏ hơn nữa (ví dụ: buttons, input fields, checkboxes, links). Chúng cũng có thể trừ tượng như colours, fonts chữ.
* Molecules: Gồm các atom kết hợp vs nhau là các phần tử bên ngoài như đơn vị (ví dụ: một input field và một button có thể kết hợp thành một khung tìm kiếm). 	\
  Molecules có thể đơn giản hoặc phức tạp, được xây dựng để tái sử dụng hoặc chỉ dụng một lần. ví dụ hình ảnh sau: Thì molecules gồm ảnh và text, progess-bar, box-ảnh.
* Organisms: Nhóm các Molecules giống nhau hoặc khác nhau để tạo thành một thành phần hoàn chỉnh của một giao diện. (Ví dụ: Header trang có thể kết hợp từ một logo, menu và khung tìm kiếm).
* Templates: Là kết hợp các organisms với nhau tạo thành các trang.
*  Pages: Là các mẫu cụ thể. Họ sẽ kiểm tra templates làm việc với nội dung thực tế như thế nào, cho phép các designers quay trở lại để chỉnh sửa các molecules, organisms, và các templates khi cần thiết.


<img src ="https://github.com/LongHuu100/FrontEnd_Architecture/blob/main/amomic.jpg" />

Kiến trúc khung của FE khi bắt đầu một project mới.

<img src ="https://github.com/LongHuu100/FrontEnd_Architecture/blob/main/fe.jpg" />
