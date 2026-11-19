# Lớp C4 của chúng mình — Hướng dẫn cập nhật

Trang không cần cài đặt hay đóng gói gì. Anh chỉ cần sửa 1 file chữ và tải ảnh lên.

## Các file

| File / thư mục | Dùng để |
|---|---|
| `index.html` | Giao diện trang (không cần sửa) |
| `du-lieu.js` | **Toàn bộ nội dung**: tên bé, ngày sinh, thư tri ân, lời kể, lời chúc, ảnh, video |
| `anh/` | Ảnh, chia theo thư mục: `dai-dien`, `khai-giang`, `trung-thu`, `20-10`, `20-11`, `co-voi-lop`, `rieng` |
| `og.png` | Ảnh hiện khi gửi link qua Zalo |
| `nen-anh.html` | Công cụ nén ảnh trước khi tải lên |

## Đưa lên GitHub lần đầu

1. Tạo repo mới, ví dụ `lop-c4`
2. Bấm **Add file → Upload files**, kéo toàn bộ các file và thư mục ở trên vào, rồi bấm **Commit**
3. Vào **Settings → Pages**, chọn nhánh `main`, bấm **Save**
4. Khoảng 1–2 phút sau là có link dạng `https://<tên-tài-khoản>.github.io/lop-c4/`

## Thêm ảnh: chỉ cần tải lên đúng thư mục, không phải sửa gì

**Nên nén ảnh trước:** mở file `nen-anh.html` (trên máy, hoặc trên trang `.../nen-anh.html` sau khi đã đưa lên GitHub) → chọn **Ảnh album** hoặc **Ảnh đại diện** → chọn ảnh → **Tải tất cả ảnh đã nén**. Ảnh 3 MB thường còn khoảng 200–300 KB, nhờ vậy trang mở nhanh trên 4G.

Trên GitHub, mở thư mục cần thêm ảnh → **Add file → Upload files** → kéo ảnh vào → **Commit changes**. Khoảng 1–2 phút sau ảnh tự hiện trên trang.

| Thư mục | Ảnh hiện ở đâu |
|---|---|
| `anh/khai-giang`, `anh/trung-thu`, `anh/20-10`, `anh/20-11`, `anh/tet`, `anh/8-3`, `anh/tong-ket` | Album của dịp đó (tab Năm học) |
| `anh/co-voi-lop` | Ảnh đầu tiên lên trang Tri ân cô, cả thư mục vào Góc của cô |
| `anh/be/12-mixue` (mỗi bé 1 thư mục) | Ảnh riêng trong Góc của con |

- **Ảnh đại diện của bé:** đặt tên ảnh bắt đầu bằng `dai-dien` (ví dụ `dai-dien.jpg`). Nếu không có ảnh nào tên như vậy thì trang lấy ảnh đầu tiên trong thư mục của bé.
- Ảnh xếp theo tên file. Muốn ảnh nào lên trước thì đặt tên `01-...`, `02-...`
- File `doc-truoc.txt` trong mỗi thư mục chỉ để giữ thư mục, không cần xóa
- Ảnh tải từ Zalo (jpg) dùng được luôn. Ảnh HEIC chụp từ iPhone thì cần đổi sang jpg trước.
- Muốn ghi chú thích cho ảnh thì thêm vào `du-lieu.js`, mục `"anh"` của dịp: `{"tep": "anh/trung-thu/1.jpg", "chu": "Các con rước đèn"}`

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
- Ảnh tải từ Zalo đã đủ nhẹ, không cần nén thêm
