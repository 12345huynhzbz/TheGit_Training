# 1.GIT LÀ GÌ?
- **Git** là một **hệ thống kiểm soát phiên bản phân tán code nguồn mở**. Nó được thiết kế để xử lý các dự án từ nhỏ đến lớn với tốc độ và hiệu quả cao. Nó được phát triển để điều phối công việc giữa các developer. Kiểm soát phiên bản cho phép chúng ta theo dõi và làm việc cùng với các thành viên trong nhóm của chúng ta tại cùng một không gian làm việc.

# 2. TẠI SAO LẠI DÙNG GIT?
- **Tiết kiệm thời gian (save time)**  
	Git là công nghệ **nhanh như chớp**. Mỗi lệnh chỉ mất vài giây để thực thi nên chúng ta có thể tiết kiệm rất nhiều thời gian so với đăng nhập vào tài khoản GitHub và tìm hiểu các tính năng của nó.
- **Làm việc ngoại tuyến (offline working)**
    Một trong những lợi ích quan trọng nhất của Git là nó hỗ trợ **làm việc ngoại tuyến**. Nếu chúng ta đang gặp phải sự cố kết nối internet, nó sẽ không ảnh hưởng đến công việc của chúng ta. Trong Git, chúng ta có thể làm hầu hết mọi thứ cục bộ. So sánh, các CVS ​​khác như SVN bị hạn chế và thích kết nối với kho lưu trữ trung tâm hơn.
- **Hoàn lại sai lầm (undo mistakes)**
	Một lợi ích bổ sung của Git là chúng ta có thể **Hoàn tác** lỗi. Đôi khi hoàn tác có thể là một lựa chọn cứu tinh cho chúng ta. Git cung cấp tùy chọn hoàn tác cho hầu hết mọi thứ.
- **Theo dõi các thay đổi (Track changes)**
    Git tạo điều kiện với một số tính năng thú vị như **Diff, Log** và **Status** , cho phép chúng ta theo dõi các thay đổi để chúng ta có thể **kiểm tra trạng thái, so sánh** các file hoặc chi nhánh của mình.

# 3. GIT CƠ BẢN
**a. Tải xuống Git**
 - Trước khi tải về Git thì bạn cần có một tài khoản [Github](https://github.com)
 - Git có sẵn tại hầu hết phiên bản của MacOS và Linus. Chính vì vậy, người dùng của hai hệ điều hành này không cần thiết phải tải xuống. Tuy nhiên đây là [cách để tải Git về trên MacOS](https://git-scm.com/download/mac)
 - Để tại về Git trên Windows cũng khá đơn giản, bạn có thể sử dụng [hướng dẫn sau tại trang chủ của Git](https://git-scm.com/download/win)
 - Để kiểm tra xem Git được tải thành công chưa bạn có thể sử dụng lệnh ```git --version``` ở terminal hoặc cmd

 b. Sử dụng Git

 **b.1 Clone một repository**
- Để clone một repository bạn mong muốn hãy sử dụng lệnh ```git clone``` đi cùng với đường link định dạng https hoặc ssh của repo mà bạn muốn clone

```
# Phương thức HTTPS
git clone https://github.com/kimlienartoftech/TheGit_Training
# Còn đây là SSH
git clone git@github.com:kimlienartoftech/TheGit_Training.git
```
 - Còn một phương thức khác là sử dụng GitCLI nhưng chúng ta sẽ không đề cập đến đây vì không phổ biến

 - Việc clone này sẽ đồng thời clone toàn bộ lịch sử chỉnh sửa của repo đó => Nếu repo có dung lượng lớn hoặc có nhiều chỉnh sửa có thể sử dụng phương thức sau 
```
git clone (đường link) --depth 1
```
 - Sau đó thì bạn có thể dùng nhiều phương thức để mở repo đó lúc này đang ở dưới dạng Folder trong máy bạn

 **b.2 Các lệnh cơ bản trong Git**
 1. Kiểm tra trạng thái branch, các file chưa được commit hoặc các file đã commit

```
git status
```

 2. Thêm thay đổi ở các tệp
```
git add (tên tệp bạn muốn thêm)
```
 - Tuy nhiên nếu số lượng file thay đổi là quá lớn bạn có thể sử dụng một trong hai lệnh sau để thêm toàn bộ file
```
git add --all
git add .
```

