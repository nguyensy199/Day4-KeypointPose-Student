# REVIEWER CHECKLIST

Vì tôi làm việc độc lập 1 mình, checklist này được dùng làm công cụ tự đánh giá (Self-Assessment).

- [x] **Format file nhãn chuẩn YOLO Pose:** Các file `.txt` có số lượng phần tử đúng (tọa độ bbox, class, 17 điểm với tọa độ x,y và cờ v).
- [x] **Không nhầm lẫn Trái/Phải (Left/Right):** Đã kiểm tra và chỉnh sửa lỗi lệch vai/hông.
- [x] **Gán cờ Visibility chính xác:** 
    - [x] Không gán `v=0` khi đối tượng vẫn nằm toàn vẹn trong ảnh.
    - [x] Đã sử dụng `v=1` cho các khớp bị vật thể hoặc cơ thể che lấp nhưng có thể đoán được vị trí.
- [x] **Điểm nằm trong bounding box:** Tất cả các điểm keypoint của một người (trừ một số ngoại lệ nhỏ vung tay/chân) đều nằm gọn trong bounding box.
- [x] **Xác định khớp Hông/Vai đồng nhất:** Có tuân theo Guideline đã thiết lập (ở giữa mép đùi và eo đối với hông).
- [x] **Khớp Cổ và Mũi:** Điểm mũi nằm chính giữa khuôn mặt, cổ ở đường cơ sở nối hai vai và đầu.
