---
description: Tạo bài blog mới cho website Tương Ớt Siêu Cay
---

# Tạo Bài Blog Mới

## Thông tin website
- **Domain**: tuongotcay.github.io
- **Thư mục blog**: `f:\tuongotcay.github.io\blog\`
- **Blog index**: `f:\tuongotcay.github.io\blog\index.html`
- **Google Analytics**: G-6JHML7VMEB
- **Thương hiệu**: Tương Ớt Siêu Cay - Bông Ớt
- **Sản phẩm**: Tương ớt nguyên chất (100% ớt, KHÔNG tỏi, KHÔNG cà chua, không chất bảo quản)
- **SĐT**: 0982722036
- **Email**: vietthanh228@gmail.com
- **Copyright**: © 2011

## Quy trình tạo bài

### 1. Nhận yêu cầu từ user
- Tiêu đề bài viết
- Chủ đề/nội dung chính (nếu user cung cấp)

### 2. Tạo file HTML bài viết
- Tên file: slug tiếng Việt không dấu, ngăn cách bằng dấu gạch ngang (ví dụ: `an-ot-co-giup-giam-can-khong.html`)
- Đặt trong thư mục `f:\tuongotcay.github.io\blog\`

### 3. Cấu trúc bài viết BẮT BUỘC

#### Head (SEO)
- `<title>` - Tiêu đề bài + "| Blog Tương Ớt Siêu Cay"
- `<meta name="description">` - Mô tả 150-160 ký tự
- `<meta name="keywords">` - 8-12 keywords liên quan, phân cách bằng dấu phẩy
- Open Graph tags (og:type, og:url, og:title, og:description, og:image)
- Twitter Card tags
- `<link rel="canonical">`
- Google Site Verification: H-1uGYQBFn_CIx4O_Q3IoRNPm06vMAwyE72Rwy6Dzlk
- CSS: `../styles.min.css` + `blog.min.css`
- Font Awesome 6.0.0
- Google Fonts: Roboto + Dancing Script
- Favicon: https://cdn-icons-png.flaticon.com/512/5495/5495490.png

#### Schema.org (trong <head>)
- **Article** schema (headline, author, datePublished, dateModified, publisher)
- **BreadcrumbList** schema (Trang Chủ > Blog > Tên bài)
- **FAQPage** schema (nếu bài có phần FAQ - thường 3 câu hỏi)

#### GA4 tracking
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-6JHML7VMEB"></script>
<script>window.dataLayer=window.dataLayer||[];function gtag(){dataLayer.push(arguments);}gtag('js',new Date());gtag('config','G-6JHML7VMEB');</script>
```

#### Body
- **Header**: Navbar với logo + 4 link (Trang Chủ, Sản Phẩm, Blog [active], Liên Hệ)
- **Blog Header**: Gradient đỏ `rgba(220,53,69,0.2)` → `rgba(255,107,107,0.1)`, breadcrumb, h1 với icon, meta (ngày, thời gian đọc, tác giả)
- **Article Content**: 
  - Nút "Quay lại danh sách bài viết"
  - Nội dung chính với h2, h3, bảng dữ liệu, info-box (success/warning/default)
  - CTA box cuối bài: gradient đỏ `#dc3545` → `#ff6b6b`, nút trắng chữ đỏ
  - Share buttons (Facebook, Twitter, Copy link)
- **Related Articles**: 3 bài viết liên quan
- **Footer**: Brand, Liên Kết Nhanh, Liên Hệ, Copyright © 2011

#### Scripts
```html
<script src="../script.min.js"></script>
<script src="blog.min.js"></script>
```

### 4. Thêm card vào blog index
- Mở file `f:\tuongotcay.github.io\blog\index.html`
- Thêm card mới vào ĐẦU danh sách `<div class="blog-grid">`
- Card gồm: image gradient, icon, category, title, excerpt, link, meta (ngày, thời gian đọc)

### 5. Kiểm tra
- File HTML hợp lệ
- Tất cả link đúng
- Schema.org đầy đủ
- Keywords phù hợp với nội dung

## Lưu ý quan trọng
- **KHÔNG** đề cập tỏi hoặc cà chua trong công thức sản phẩm
- Sản phẩm là tương ớt **nguyên chất** chỉ từ ớt
- Luôn có CTA dẫn về trang sản phẩm `../index.html#products`
- Dùng dark theme (trang web dùng dark mode)
- Icon dùng Font Awesome 6
- Bảng dùng class `article-table`, info box dùng class `info-box` (+ `success`/`warning`)
- Ngày publish dùng ngày hiện tại
