# Web Learning - HTML Practice Website

Website thực hành HTML/CSS cơ bản, gồm các trang minh họa form, multimedia và Semantic HTML5.

## Thông tin sinh viên

- Họ tên: Đào Quốc Đại
- MSSV: 20235290
- Domain: `dqd20235290.io.vn`
- Hosting: InfinityFree

## Cấu trúc project

```text
website/
├── index.html
├── register.html
├── media.html
├── index_new.html
├── prompt_CRAFT_semantic_html5.md
├── images/
└── media/
```

## Các trang chính

### `index.html`
Trang chủ của website.

Nội dung chính:
- Header
- Thanh điều hướng
- Hero section
- Sidebar
- Các card giới thiệu nội dung
- Phần giới thiệu HTML/CSS
- Footer

Trang này chủ yếu sử dụng các thẻ `div` để làm phiên bản ban đầu trước khi refactor sang Semantic HTML5.

### `register.html`
Trang đăng ký nhận thông tin.

Form có sử dụng:
- `input type="text"`
- `input type="email"`
- `input type="tel"`
- `input type="date"`
- `radio`
- `checkbox`
- `select`
- `textarea`
- `button`

### `media.html`
Trang đa phương tiện.

Các thẻ HTML5 được minh họa:
- `figure`
- `figcaption`
- `audio`
- `video`
- `section`
- `article`

### `index_new.html`
Phiên bản refactor của `index.html` sang Semantic HTML5.

Một số thay đổi chính:

```text
<div id="header">  -> <header id="header">
<div id="nav">     -> <nav id="nav">
<div id="sidebar"> -> <aside id="sidebar">
<div id="content"> -> <main id="content">
<div id="footer">  -> <footer id="footer">
```

Mục tiêu là cải thiện cấu trúc tài liệu, khả năng đọc mã, accessibility và SEO cơ bản nhưng vẫn giữ nguyên nội dung và bố cục so với `index.html`.

## Prompt AI

File `prompt_CRAFT_semantic_html5.md` chứa prompt theo công thức CRAFT dùng để yêu cầu AI refactor `index.html` sang Semantic HTML5.

CRAFT gồm:

- C - Context
- R - Role
- A - Action
- F - Format
- T - Tone / Target

## Cách chạy

Không cần cài thêm thư viện.

Có thể mở trực tiếp:

```text
index.html
```

bằng trình duyệt.

Hoặc chạy qua extension Live Server trong Visual Studio Code.

## Điều hướng

Các trang được liên kết với nhau qua thanh menu:

```text
Trang chủ -> index.html
Đăng ký -> register.html
Đa phương tiện -> media.html
HTML5 Semantic -> index_new.html
```

## Triển khai

Sau khi hoàn thiện, upload toàn bộ file website vào thư mục:

```text
dqd20235290.io.vn/htdocs/
```

trên InfinityFree.

File `index.html` cần nằm trực tiếp trong `htdocs` để website có thể mở từ domain chính.

## Ghi chú

Các file `media.html` hiện có thể sử dụng media mẫu trực tuyến. Nếu muốn chạy hoàn toàn offline, tải ảnh/audio/video về các thư mục `images/` và `media/`, sau đó sửa lại đường dẫn `src`.
