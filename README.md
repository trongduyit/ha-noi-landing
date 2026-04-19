# Hà Nội Dịu Dàng 🌸

Landing page nghệ thuật — Album ảnh Hà Nội dịu dàng, có upload ảnh cá nhân và video nền.

## ✨ Tính năng

- 🎬 Video nền hero tự động phát (muted, loop)
- 📸 42 ảnh dataset Hà Nội hiển thị trong album
- 📷 Upload ảnh cá nhân — lưu trong trình duyệt (IndexedDB)
- 🎵 Nhạc nền toggle bật/tắt (tùy chỉnh file nhạc)
- 🖼️ Lightbox xem ảnh lớn — có prev/next
- 📱 Responsive — đẹp trên mobile, tablet, desktop

## 🎨 Design

- Màu sắc: hồng phấn (#EBC8D8) + xanh lavender (#B5C7D3) + trắng ngà (#FAF7F4)
- Font: Playfair Display (heading) + Nunito (body)
- Animation: scroll reveal, hover zoom, lightbox fade

## 📁 Cấu trúc

```
hanoi-landing/
├── index.html              ← Trang chính (tất cả CSS/JS inline)
├── assets/
│   ├── images/             ← 42 ảnh dataset
│   ├── video/
│   │   └── background.mp4  ← Video nền hero
│   └── music/
│       └── music.mp3       ← Nhạc nền (thêm file của bạn)
└── README.md
```

## 🚀 Chạy local

**Cách 1 — Mở trực tiếp:**
```bash
# Windows: double-click index.html hoặc
start index.html

# macOS:
open index.html

# Linux:
xdg-open index.html
```

**Cách 2 — Local server (khuyên dùng để test đầy đủ):**
```bash
# Python 3
python -m http.server 8080

# Sau đó mở: http://localhost:8080
```

## 🌐 Deploy lên Render.com (Static)

1. **Tạo repo GitHub** chứa toàn bộ project `hanoi-landing/`
2. Đăng nhập [Render.com](https://render.com) → **New → Static Site**
3. Kết nối repo GitHub, chọn branch `main`
4. **Build Command:** (để trống — không cần)
5. **Publish Directory:** `.`
6. Click **Create Static Site** → done!

> ⚠️ Nếu có file nhạc, đặt vào `assets/music/music.mp3` trước khi deploy.

## 🎵 Thêm nhạc nền

Đặt file MP3 vào: `assets/music/music.mp3`

## 💾 Lưu trữ

Ảnh upload được lưu trong **IndexedDB** của trình duyệt — không tốn server, dữ liệu riêng tư. Xóa dữ liệu trình duyệt sẽ mất ảnh đã upload.

---

*Một góc Hà Nội trong ánh nắng mùa thu* 🌸