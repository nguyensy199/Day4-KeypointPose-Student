# Nhận xét bài của Partner (Review Partner)

**Người review:** [Cá nhân]
**Người bị review:** [Cá nhân]

*Ghi chú: Vì làm việc độc lập 1 mình, đây là nhận xét cho chính tập dữ liệu tôi vừa gán.*

### 1. Điểm tốt
- Đã gán nhãn đầy đủ 17 khớp trên các hình ảnh huấn luyện.
- Hiểu được định dạng YOLO pose (.txt).
- Khớp mũi, mắt, tai thường rất chuẩn xác.

### 2. Điểm cần cải thiện
- Việc ước lượng các điểm bị che khuất (v=1) đôi khi vẫn còn thiếu tự tin, dẫn đến gán nhầm thành v=0. Đặc biệt ở các tư thế phức tạp hoặc hai người chồng chéo lên nhau.
- Cần chú ý kỹ hơn quy tắc không đảo ngược trái/phải, một lỗi đã bị script check bắt được ở `train_02`.

### 3. Đánh giá chung
- Pass. Sau khi sửa các cảnh báo từ script check, dữ liệu có thể đưa vào để tiếp tục huấn luyện vòng lặp data.
