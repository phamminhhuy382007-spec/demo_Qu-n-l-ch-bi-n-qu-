# Senspices — Quản lý chế biến quế

Ứng dụng web một trang giúp theo dõi các lô chế biến quế, sản lượng thành phẩm và tỷ lệ hao hụt.

## Chạy ứng dụng

Ứng dụng dùng HTML, CSS, JavaScript thuần và Tailwind CSS qua CDN. Mở `index.html` trên trình duyệt có kết nối Internet. Hoặc chạy máy chủ tĩnh trong thư mục dự án:

```bash
python3 -m http.server 8000
```

Sau đó mở `http://localhost:8000`.

## Tính năng

- Dashboard tổng hợp nguyên liệu đầu vào, thành phẩm và tỷ lệ hao hụt.
- Ba lô mẫu Yên Bái / Hà Nam được khởi tạo khi chạy lần đầu.
- Tính toán trực tiếp; dữ liệu lô được lưu trong `localStorage` của trình duyệt hiện tại.
- Cảnh báo đỏ cho lô có tỷ lệ hao hụt trên 15%.
- Xuất lịch sử thành CSV có BOM để mở bằng Excel.

Dữ liệu được lưu cục bộ trong trình duyệt, không đồng bộ giữa các thiết bị hoặc trình duyệt khác nhau.
