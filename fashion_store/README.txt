FASHIONLY — WEBSITE BÁN QUẦN ÁO (DEMO HCI)

CÁCH CHẠY:
1. Giải nén Fashionly_Web_HCI.zip.
2. Mở thư mục fashion_store.
3. Nháy đúp file index.html để mở trên Chrome/Edge.
4. Nếu muốn chạy như một website local: mở Terminal tại thư mục này và chạy:
   python -m http.server 8000
   Sau đó mở http://localhost:8000

CÁC CHỨC NĂNG:
- Trang chủ, banner, voucher, danh sách sản phẩm.
- Tìm kiếm, lọc danh mục, sắp xếp theo giá / giảm giá.
- Chi tiết sản phẩm: chọn màu, size, số lượng.
- Giỏ hàng: thêm, xóa, tăng/giảm số lượng, tính tiền.
- Checkout: thông tin nhận hàng, COD hoặc chuyển khoản mô phỏng.
- Xác nhận đặt hàng bằng popup, màn hình thành công.
- Theo dõi đơn hàng, hủy đơn khi còn chờ xác nhận.
- Trang Admin riêng (admin.html): đăng nhập demo, xem thống kê, thêm/sửa/xóa sản phẩm, tìm kiếm và lọc danh mục.
- Quản lý đơn: xem chi tiết, xác nhận -> giao hàng -> hoàn thành; từ chối đơn.
- Tài khoản đăng ký / đăng nhập demo.
- Responsive trên laptop, tablet, điện thoại.

THỬ LUỒNG:
Trang chủ -> sản phẩm -> chọn size + màu -> thêm giỏ -> giỏ hàng
-> thanh toán -> đặt hàng -> xác nhận -> theo dõi đơn
-> Admin (truy cập admin.html hoặc link ở trang Tài khoản)
-> đăng nhập tài khoản demo: admin@fashionly.demo / admin123
-> thêm/sửa/xóa sản phẩm hoặc xử lý đơn -> quay lại cửa hàng để xem thay đổi.

MÃ VOUCHER DEMO:
FASHION100 (giảm 100.000đ, đơn từ 799.000đ)
FASHION50 (giảm 50.000đ, đơn từ 399.000đ)
FASHION30 (giảm 30.000đ, đơn từ 399.000đ)
Miễn phí ship từ 499.000đ; dưới mức này ship 30.000đ.

LƯU Ý:
- Demo front-end, dữ liệu lưu bằng localStorage của trình duyệt.
- Chưa có backend, cơ sở dữ liệu server, tài khoản bảo mật hoặc cổng thanh toán thật.
- Admin dùng biểu mẫu đăng nhập demo, không phải cơ chế phân quyền/bảo mật máy chủ.
- Danh mục sản phẩm Admin được lưu vào localStorage và hiển thị khi tải lại cửa hàng.
- Chức năng ảnh sản phẩm hỗ trợ chọn ảnh mẫu hoặc nhập URL HTTPS; không tải ảnh lên máy chủ.
- Đơn hàng chỉ đồng bộ giữa các tab trong cùng trình duyệt/cùng địa chỉ web,
  không tự đồng bộ giữa các máy khác nhau.
- Ảnh sản phẩm/banner được cắt từ ảnh chụp Figma do người dùng cung cấp,
  nên chất lượng thấp hơn file ảnh gốc. Có thể thay trong thư mục assets.
- Nội dung, giá và sản phẩm trong web là dữ liệu demo.
