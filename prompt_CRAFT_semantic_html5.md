# Prompt CRAFT – Refactor `index.html` sang Semantic HTML5

## C – Context

Tôi có một trang web `index.html` đã hoàn thiện về nội dung, bố cục và CSS.  
Trang hiện tại đang sử dụng nhiều thẻ `div` để chia các khu vực lớn như header, navigation, sidebar, nội dung chính và footer.

Yêu cầu của bài tập là tạo một file mới tên `index_new.html`, giữ nguyên bố cục, nội dung và giao diện của `index.html`, nhưng refactor cấu trúc sang các thẻ Semantic HTML5 nhằm cải thiện SEO cơ bản và làm mã HTML rõ nghĩa hơn.

---

## R – Role

Bạn là một lập trình viên Front-end có kinh nghiệm về:

- HTML5 Semantic
- SEO cơ bản
- Accessibility
- Refactor HTML/CSS
- Giữ tính tương thích với CSS hiện có

---

## A – Action

Hãy phân tích toàn bộ mã nguồn `index.html` được cung cấp và thực hiện các yêu cầu sau:

1. Chuyển các thẻ `div` dùng để biểu diễn khu vực có ý nghĩa ngữ nghĩa sang thẻ Semantic HTML5 phù hợp, ví dụ:
   - `header`
   - `nav`
   - `main`
   - `section`
   - `article`
   - `aside`
   - `footer`

2. Không thay đổi nội dung văn bản của trang.

3. Không thay đổi thứ tự các thành phần trên trang.

4. Không thay đổi bố cục và giao diện hiện tại.

5. Giữ nguyên các `id` và `class` cần thiết để CSS hiện tại tiếp tục hoạt động.

6. Không đổi tên file CSS, đường dẫn liên kết, hình ảnh hoặc các liên kết điều hướng.

7. Không bắt buộc phải thay mọi `div`.
   Những `div` chỉ dùng làm container phục vụ bố cục hoặc styling có thể được giữ lại nếu không có thẻ semantic phù hợp.

8. Khi chuyển đổi, ưu tiên ý nghĩa của nội dung:
   - phần đầu trang → `header`
   - menu điều hướng → `nav`
   - nội dung chính → `main`
   - nội dung phụ/sidebar → `aside`
   - từng nội dung độc lập → `article`
   - từng khu vực nội dung theo chủ đề → `section`
   - chân trang → `footer`

9. Đảm bảo file sau khi refactor vẫn là HTML5 hợp lệ và hiển thị gần như giống hệt `index.html` ban đầu.

10. Có thể bổ sung các thuộc tính hỗ trợ accessibility hoặc semantic như `aria-label` nếu hợp lý, nhưng không được làm thay đổi giao diện.

---

## F – Format

Trả về kết quả theo đúng thứ tự sau:

1. Toàn bộ mã nguồn hoàn chỉnh của file `index_new.html` trong một code block HTML.
2. Sau đó liệt kê ngắn gọn các thay đổi chính theo dạng:

```text
<div id="header">  → <header id="header">
<div id="nav">     → <nav id="nav">
<div id="sidebar"> → <aside id="sidebar">
<div id="content"> → <main id="content">
<div id="footer">  → <footer id="footer">
```

3. Giải thích ngắn gọn vì sao các thẻ Semantic HTML5 này tốt hơn về:
   - cấu trúc tài liệu
   - khả năng đọc mã
   - accessibility
   - SEO cơ bản

---

## T – Tone / Target

- Mã nguồn rõ ràng, dễ đọc.
- Tuân thủ chuẩn HTML5.
- Không tự ý thiết kế lại giao diện.
- Không thêm hoặc xóa nội dung.
- Không phá CSS hiện tại.
- Ưu tiên semantic hợp lý hơn là thay thẻ một cách máy móc.
- Kết quả phải có thể lưu trực tiếp thành file `index_new.html` và chạy ngay.

---

## Prompt hoàn chỉnh để đưa cho AI

```text
Tôi có một trang web index.html đã hoàn thiện về nội dung, bố cục và CSS. Trang hiện đang sử dụng nhiều thẻ div để chia các khu vực lớn như header, navigation, sidebar, nội dung chính và footer.

Bạn là một lập trình viên Front-end có kinh nghiệm về HTML5 Semantic, SEO cơ bản, accessibility và refactor HTML/CSS.

Hãy phân tích toàn bộ mã nguồn index.html tôi cung cấp và refactor sang Semantic HTML5 với các yêu cầu sau:

- Chuyển các div có ý nghĩa ngữ nghĩa sang các thẻ phù hợp như header, nav, main, section, article, aside và footer.
- Giữ nguyên toàn bộ nội dung văn bản.
- Giữ nguyên thứ tự các thành phần.
- Giữ nguyên bố cục và giao diện.
- Giữ nguyên các id và class cần thiết để CSS hiện tại tiếp tục hoạt động.
- Không đổi tên file CSS, đường dẫn hình ảnh hoặc liên kết.
- Không bắt buộc phải thay mọi div; các div chỉ dùng làm container hoặc phục vụ styling có thể giữ lại.
- Ưu tiên semantic đúng ý nghĩa của nội dung thay vì thay thẻ một cách máy móc.
- Có thể thêm aria-label hoặc thuộc tính accessibility nếu hợp lý nhưng không làm thay đổi giao diện.
- Đảm bảo HTML5 hợp lệ và trang sau khi refactor hiển thị gần như giống hệt index.html ban đầu.

Đầu ra:
1. Trả về toàn bộ mã HTML hoàn chỉnh của index_new.html trong một code block.
2. Liệt kê các thay đổi chính theo dạng thẻ cũ → thẻ semantic mới.
3. Giải thích ngắn gọn lợi ích của việc refactor đối với cấu trúc tài liệu, khả năng đọc mã, accessibility và SEO cơ bản.

Đây là mã nguồn index.html cần refactor:

[PASTE TOÀN BỘ NỘI DUNG index.html VÀO ĐÂY]
```
