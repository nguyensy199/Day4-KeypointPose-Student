# Visibility Report

## 1. Tóm tắt số lượng cờ
Dựa trên kết quả chạy script `tools/check_pose_labels.py`:
- Số lượng file nhãn (train): 20 file
- Số lượng skeleton (người): 27 skeleton
- **v=2 (Nhìn rõ):** 313
- **v=1 (Bị che khuất, nằm trong hình):** 119
- **v=0 (Ngoài khung hình):** 27

## 2. Các lỗi/cảnh báo được phát hiện
- `train_02.txt:1`: `left_shoulder/right_shoulder` nằm ngược chiều so với hai mắt. Dấu hiệu đảo trái/phải.
- `train_02.txt:1`: `left_hip/right_hip` nằm ngược chiều so với hai mắt.
- `train_04.txt:1` & `train_04.txt:2`: Có các khớp `v=0` trong khi cả người nằm gọn giữa ảnh. Đáng lẽ phải là `v=1`.
- `train_10.txt:1` & `train_11.txt:1`: Tương tự, có các khớp `v=0` khi người nằm gọn trong ảnh, cần đổi về `v=1`.

## 3. Hành động khắc phục
- Rà soát lại file `train_02.txt`, sửa lại trái/phải đối với vai và hông.
- Đổi lại `v=0` thành `v=1` ở các khung hình `train_04`, `train_10`, `train_11` tại các vị trí người không bị cắt bởi rìa ảnh nhưng đang bị đánh dấu ngoài khung hình.
