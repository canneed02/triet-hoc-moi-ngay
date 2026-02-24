# Triết Học Mỗi Ngày - Hướng Dẫn Đăng Bài

## 3 Cách Đăng Bài (Từ Dễ Đến Pro)

---

### Cách 1: GitHub Editor (Dễ Nhất)

Không cần cài gì, chỉ cần trình duyệt:

1. Vào https://github.com/canneed02/triet-hoc-moi-ngay
2. Bấm phím `.` trên bàn phím
3. Trình duyệt thành code editor
4. Tạo file mới hoặc copy file cũ để edit
5. Bấm "Commit changes" → Done!

**Ưu:** Không cần cài đặt  
**Nhược:** Phải biết chút HTML

---

### Cách 2: Script Tạo Bài (Cho Terminal)

```bash
cd ~/.openclaw/workspace/essays-blog
python3 create_post.py
```

Script sẽ hỏi:
- Tiêu đề bài viết
- Mô tả ngắn  
- Nội dung (gõ thoải mái)

Sau đó tự tạo file .html với format chuẩn.

**Ưu:** Format tự động đẹp  
**Nhược:** Phải chạy lệnh

---

### Cách 3: Admin Page với Decap CMS (Pro Nhất)

Để có trang `/admin` như Word:

1. Cần thêm OAuth app trên GitHub
2. Hoặc dùng Netlify deploy thay vì GitHub Pages

Liên hệ admin để setup chi tiết.

---

## Quy Trình Đăng Bài Chuẩn

### Bước 1: Tạo file bài viết
```bash
# Cách nhanh: copy file cũ
cp about.html bai-moi.html
```

### Bước 2: Sửa nội dung
- Giữ nguyên phần `<style>` và `<script>`
- Sửa phần nội dung trong `<body>`

### Bước 3: Thêm vào trang chủ
Mở `index.html` và thêm:
```html
<article>
    <div class="meta">
        <time class="date" datetime="2026-02-25">25/02/2026</time>
        <span class="read-time">• 5 phút đọc</span>
    </div>
    <h2><a href="bai-moi.html">Tiêu đề bài</a></h2>
    <p>Mô tả ngắn...</p>
</article>
```

### Bước 4: Commit & Push
```bash
git add .
git commit -m "Thêm bài: Tiêu đề"
git push origin master
```

---

## Liên Kết Hữu Ích

- **Trang web:** https://canneed02.github.io/triet-hoc-moi-ngay/
- **GitHub repo:** https://github.com/canneed02/triet-hoc-moi-ngay
- **Editor online:** https://github.com/canneed02/triet-hoc-moi-ngay/edit/master
