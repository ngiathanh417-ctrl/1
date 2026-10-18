# 💌 Thiệp 20/10 – Gửi Em Yêu

Thiệp chúc mừng 20/10 dạng trang web một trang: sao băng, pháo hoa trái tim, vòng tròn phép thuật, phong thư và lá thư gõ chữ, có nhạc nền.

## Cấu trúc

```
index.html        # toàn bộ giao diện, hiệu ứng và lời chúc
assets/music.mp3  # nhạc nền (phát khi mở thiệp hoặc lần chạm đầu tiên)
.nojekyll         # để GitHub Pages phục vụ file nguyên trạng
```

## Đưa lên GitHub và tạo đường link (GitHub Pages)

1. Tạo repository mới trên GitHub (ví dụ `thiep-20-10`).
2. Đẩy mã nguồn lên:
   ```bash
   git init
   git add .
   git commit -m "Thiệp 20/10"
   git branch -M main
   git remote add origin https://github.com/<tên-tài-khoản>/thiep-20-10.git
   git push -u origin main
   ```
   Hoặc vào repository → **Add file → Upload files** rồi kéo thả toàn bộ nội dung thư mục này.
3. Vào **Settings → Pages**, ở mục *Build and deployment* chọn **Deploy from a branch**, nhánh `main`, thư mục `/ (root)` rồi bấm **Save**.
4. Đợi khoảng 1–2 phút, link thiệp sẽ có dạng `https://<tên-tài-khoản>.github.io/thiep-20-10/`.

## Chỉnh sửa nhanh

- **Lời chúc:** tìm `typeP1`, `typeP2` trong `index.html`.
- **Cách xưng hô, tiêu đề, chữ ký:** tìm `Em Yêu`, `Người thương của em`.
- **Đổi nhạc:** thay file `assets/music.mp3` (giữ nguyên tên file).
- **Ép mức hiệu ứng cho máy yếu:** thêm `?q=low` vào cuối link.

## Lưu ý

- Repository công khai thì ai có link cũng xem được thiệp.
- Nhạc nền là bài hát có bản quyền; nếu để repository công khai, hãy cân nhắc trước khi đăng.
- Trình duyệt thường chặn nhạc tự phát khi chưa chạm vào trang, nên nhạc có thể chỉ bắt đầu sau lần chạm đầu tiên.
