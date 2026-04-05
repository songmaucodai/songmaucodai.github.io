# Trạm Điều Hướng

Kho lưu trữ này chứa trang tĩnh (`index.html`) đóng vai trò làm biển báo thông báo việc di dời tên miền của Sống Màu Cỏ Dại.

### Cơ chế hoạt động của index.html

Trang web được thiết kế theo phong cách tối giản, sử dụng giao diện Terminal mô phỏng. Nó không chứa bất kỳ thẻ liên kết (hyperlink) ngoại tuyến nào. 

Thay vào đó, mã nguồn sử dụng một kịch bản JavaScript (hiệu ứng máy đánh chữ) để hiển thị quá trình giải mã trực tiếp trên màn hình. Kịch bản này gọi hàm `atob()` để dịch ngược chuỗi Base64 định sẵn:

`c29uZ21hdWNvZGFpLmNvbQ==`

Kết quả trả về trên Terminal chính là địa chỉ văn bản của "Nhà chính thức" mới. Cách tiếp cận này giúp trang web duy trì trạng thái đóng kín hoàn toàn (Air-gapped) và an toàn trước các trình quét liên kết tự động.
