# Lớp C4 của chúng mình — Hướng dẫn cập nhật

Trang không cần cài đặt hay đóng gói gì. Anh chỉ cần sửa 1 file chữ và tải ảnh lên.

## Các file

| File / thư mục | Dùng để |
|---|---|
| `index.html` | Giao diện trang (không cần sửa) |
| `du-lieu.js` | Chữ: tên bé, ngày sinh, thư tri ân, lời kể, lời chúc, video |
| `nen-anh.html` | Công cụ nén ảnh |
| `og.png` | Ảnh hiện khi gửi link qua Zalo |
| `anh/` | Ảnh, mỗi dịp một thư mục: `khai-giang`, `trung-thu`, `20-10`, `tam-biet-nam-khanh`, `20-11`, `tet`, `8-3`, `tong-ket`, `co-voi-lop` |

## Đưa lên GitHub lần đầu

1. Repo: `c4uyno2627.github.io`
2. Giải nén bộ trang. Trên máy tính, mở repo → **Add file → Upload files** → kéo **4 file và thư mục `anh`** vào (kéo thả, không dùng nút chọn file) → **Commit changes**
3. Vào **Settings → Pages**, chọn nhánh `main`, bấm **Save**
4. Khoảng 1–2 phút sau trang chạy tại https://c4uyno2627.github.io

## Thêm ảnh

**Cách 1: thả vào thư mục**
- Trên GitHub mở thư mục, ví dụ `anh/20-11` → **Add file → Upload files** → kéo ảnh vào → **Commit changes**
- Ảnh cô với các con: thư mục `anh/co-voi-lop` (ảnh đầu tiên lên trang Tri ân)
- **Ảnh riêng của bé:** tạo thư mục mới tên đúng như `"tenAnh"` của bé, ví dụ `anh/mixue`, `anh/bao-ngoc`, `anh/nh-tue-nhi`. Cách tạo: **Add file → Create new file**, gõ `anh/mixue/doc-truoc.txt`, gõ 1 chữ bất kỳ rồi **Commit**
- Ảnh tên `dai-dien.jpg` trong thư mục của bé là **ảnh đại diện** trên cây. Không có thì trang lấy ảnh đầu tiên.

**Cách 2: không cần thư mục**
- Dùng `nen-anh.html`: chọn ảnh của ai → chọn ảnh → tải về. Ảnh được tự đặt tên (ví dụ `20-11-20261120-0800-01.jpg`, `mixue-dai-dien.jpg`), tải lên đâu trong repo cũng được.

Hai cách dùng lẫn nhau được. Ảnh xếp theo tên file.

**Mẹo:** trên máy tính (Chrome/Edge) có thể **kéo cả thư mục** vào ô Upload files, GitHub giữ nguyên thư mục. Còn nút "choose your files" chỉ chọn được file lẻ, không chọn được thư mục.

**Nên nén ảnh trước** bằng `nen-anh.html` (ảnh 3 MB còn khoảng 200–300 KB) để trang mở nhanh trên 4G.

## Thêm lời kể, lời chúc, video

```
"keChuyen": [
 {"be": "Bảo Ngọc", "loi": "Tối nào con cũng xếp gấu bông thành hàng rồi điểm danh như cô."}
],
"loiChuc": [
 {"ai": "Bố mẹ bé Mixue", "loi": "Cảm ơn hai cô đã yêu thương các con."}
],
"video": "https://youtu.be/..."
```

## Lưu ý khi sửa du-lieu.js

- Giữ đúng **dấu ngoặc kép** `" "`, **dấu phẩy** giữa các mục, và **ngoặc vuông** `[ ]`
- Sửa xong thì bấm **Commit changes**, khoảng 1 phút sau trang tự cập nhật
- Nếu trang bị trắng sau khi sửa thì gần như chắc chắn là thiếu hoặc thừa một dấu phẩy, dấu ngoặc. Gửi file cho Claude kiểm tra.

## Mẹo

- Xem trang như vào đúng một ngày nào đó: thêm `?ngay=2026-11-20` vào cuối link
- Mã vào trang của bé là **ngày và tháng sinh** (4 số), lấy từ ô `"sn"`. Mã của 2 cô là `"maCo"`.
