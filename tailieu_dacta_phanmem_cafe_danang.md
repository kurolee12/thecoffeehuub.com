# ĐẶC TẢ HỆ THỐNG PHẦN MỀM QUẢN LÝ QUÁN CAFE (CAM LE - DA NANG POS)

## 1. TỔNG QUAN HỆ THỐNG & NGUYÊN TẮC THIẾT KẾ CỐT LÕI
- **Mục tiêu**: Phần mềm vận hành quán cafe tại Quận Cẩm Lệ, Đà Nẵng - Tối ưu cho môi trường bán lẻ dịch vụ đồ uống nhanh, cao điểm sáng/tối.
- **Quy tắc 3 Chạm (Speed First)**: Chọn Bàn -> Chọn Món + Topping/Modifier -> Nhận Tiền/In Hóa Đơn trong < 3 giây.
- **Kiến trúc Offline-First (Local-First Sync)**: 
  - Lưu trữ cơ sở dữ liệu IndexedDB/SQLite cục bộ tại máy POS (Native Desktop/Electron/PWA Cache).
  - Tự động hoạt động 100% khi mất cáp mạng hay Wi-Fi chập chờn.
  - Tự động đồng bộ hai chiều (Bi-directional delta sync) lên Cloud ngay khi có kết nối trở lại.
- **Tương tác phần cứng ngoại vi**: Tích hợp trực tiếp máy in hóa đơn nhiệt qua giao thức ESC/POS (USB/LAN/Bluetooth), kích hoạt két đựng tiền (cash drawer RJ11).

---

## 2. CÁC PHÂN HỆ CHỨC NĂNG CỐT LÕI

### 2.1. Quản lý Thực đơn & Modifier Linh hoạt
- Danh mục đa tầng: Cà phê Việt, Cà phê Máy, Trà trái cây, Đá xay, Bánh & Ăn vặt.
- Nhóm tùy biến (Modifiers/Customization):
  - Đường: 100%, 70%, 50%, 30%, Không đường.
  - Đá: Bình thường, Ít đá, Không đá, Đá riêng.
  - Topping: Thạch cà phê, Trân châu phô mai, Kem cheese, Sữa yến mạch (+10k).
  - Ghi chú thao tác nhanh: "Mang về", "Không ống hút nhựa", "Uống nóng".

### 2.2. Quản lý Bàn & Sơ đồ Quán (Table Layout & Order Flow)
- Sơ đồ khu vực trực quan: Tầng trệt (Trong nhà), Sân vườn ngoài trời, Tầng 1 (Máy lạnh).
- Trạng thái bàn thời gian thực (Real-time Color Code):
  - Xanh: Bàn trống.
  - Vàng: Đang order/Chờ pha chế.
  - Đỏ: Khách đang ngồi (Hiển thị thời gian & tổng tiền tạm tính).
  - Tím: Đã in tạm tính/Chờ thanh toán.
- Thao tác nhanh: Gộp bàn, Chuyển bàn, Tách bill, Tạm giữ đơn mang về (Takeaway).

### 2.3. Quản lý Định lượng pha chế & Kho nguyên liệu (Recipe & Inventory)
- Khai báo Recipe trừ kho tự động khi hoàn tất đơn:
  - Ví dụ Cà phê Phin Sữa: 25g hạt Robusta Cẩm Lệ xay + 30ml sữa đặc Ông Thọ + 1 phin nước sôi.
- Cảnh báo tồn kho an toàn: Báo đỏ khi sữa đặc < 5 hộp, cà phê bột < 2kg.
- Quản lý nhà cung cấp, kiểm kê hao hụt thực tế cuối ngày.

### 2.4. Báo cáo Doanh thu & Chỉ số Thời gian thực
- Dashboard điều hành cho Chủ quán:
  - Doanh thu theo giờ, phân bổ khung giờ cao điểm (7h - 9h sáng, 19h - 21h tối).
  - Top món bán chạy nhất (Best sellers) & món ế cần điều chỉnh recipe/giá.
  - Báo cáo phương thức thanh toán: Tiền mặt, Quét mã VietQR/MoMo, Chuyển khoản.

### 2.5. Khách hàng thân thiết & CRM
- Tích điểm theo số điện thoại (1 điểm cho mỗi 10.000 VNĐ).
- Hạng thẻ: Đồng, Bạc, Vàng. Giảm trực tiếp 10% - 15% khi quét số điện thoại.
- Voucher sinh nhật, khuyến mãi khung giờ vàng.

### 2.6. Phân quyền chặt chẽ & Audit Log (Chống thất thoát)
- **Thu ngân / Order**: Nhận món, in bill, hủy món trước khi gửi bar (cần OTP quản lý nếu hủy sau khi pha).
- **Barista (KDS màn hình bếp/pha chế)**: Nhận order, đổi trạng thái làm xong.
- **Quản lý**: Giảm giá bill, mở két tiền khẩn cấp, xuất báo cáo ca.
- **Chủ quán**: Quản lý giá vốn, doanh số tổng, log can thiệp hệ thống.
