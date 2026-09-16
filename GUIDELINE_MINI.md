# GUIDELINE MINI

## Luật lệ thống nhất nhóm (Làm việc cá nhân)

Vì bài này tôi làm 1 mình, các quy tắc này được tôi tự thống nhất và áp dụng nhất quán trong quá trình gán nhãn:

1.  **Cách ước lượng điểm hông/hip:**
    *   Xác định phần eo và mép đùi ngoài. Điểm hông được ước lượng nằm ở giữa nếp lấp phần đùi và thân trên.
    *   Nếu bị che khuất bởi áo dài hoặc vật thể, dùng tỷ lệ cơ thể (đầu - cổ - xương sống) để ước lượng vị trí tương đối và gán cờ visibility là `v=1`.

2.  **Cách ước lượng điểm vai/shoulder:**
    *   Đối chiếu với chiều của hai mắt để tránh tình trạng gán ngược trái/phải (như đã cảnh báo trong log kiểm tra: `left_shoulder/right_shoulder nằm ngược chiều so với hai mắt`).

3.  **Quy tắc về cờ Visibility (v):**
    *   `v=2`: Nhìn thấy rõ ràng.
    *   `v=1`: Bị che khuất (bởi một phần cơ thể khác hoặc vật thể) nhưng chắc chắn điểm đó vẫn nằm trong khung hình (như cảnh báo: `có 4 khớp v=0 trong khi cả người nằm gọn giữa ảnh. Khớp không ra khỏi khung được thì phải là v=1`).
    *   `v=0`: Điểm hoàn toàn nằm ngoài khung hình (out of frame).

4.  **Kiểm tra tính trái phải:**
    *   Luôn chú ý tính đồng nhất trái phải đối xứng. Kiểm tra kỹ tay/chân và vai/hông. Đảm bảo đúng góc nhìn của camera so với đối tượng.
