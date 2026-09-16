# Báo cáo kiểm chéo Visibility

*Lưu ý: Bài tập này được thực hiện độc lập (1 mình), nên không có bước kiểm chéo với partner.*

## Tự kiểm tra chéo (Self-Review)

Thay vì kiểm chéo với bạn cùng nhóm, tôi đã tiến hành kiểm chéo vòng 2 cho chính dữ liệu của mình bằng cách:
1.  **Dùng tool visualize:** Chạy script `tools/visualize_pose.py` để xem các điểm gán lên ảnh có hợp lý không.
2.  **Rà soát cảnh báo:** Các cảnh báo về `v=0` (nhầm với `v=1` khi ở trong khung hình) đã được chú ý và đưa vào sửa đổi theo đúng `visibility_report.md`.
3.  **Xác nhận độ lệch cờ:** Hầu hết lỗi nằm ở chỗ hiểu nhầm `v=0` (không nhìn thấy, nằm ngoài ảnh) và `v=1` (bị che khuất nhưng vẫn ở trong ảnh).
