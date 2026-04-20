# learn_word

Ứng dụng học từ vựng Nhật (HTML + React CDN) chạy tĩnh và có thể deploy bằng GitHub Pages.

## Chạy local

Lưu ý: không mở trực tiếp bằng `file://` nếu muốn app tự đọc JSON bằng `fetch`.

```bash
python3 -m http.server 5500
```

Mở: `http://localhost:5500/test4.html`

## Dữ liệu bài học

App có 2 cách nạp dữ liệu:

- Nạp trực tiếp từ các file JSON đã push lên repo (dropdown "Nạp bài trực tiếp từ repo").
- Upload file JSON từ máy local.

## Deploy GitHub Pages

1. Push code lên nhánh `main`.
2. Vào GitHub repo -> Settings -> Pages.
3. Source: Deploy from a branch.
4. Branch: `main`, folder: `/ (root)`.
5. Truy cập URL dạng `https://<username>.github.io/<repo>/test4.html`.

## Cấu trúc chính

- `test4.html`: app chính.
- `*.json`: dữ liệu từ vựng.
