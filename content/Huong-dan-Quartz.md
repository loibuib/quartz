---
title: Hướng dẫn viết bài với Quartz & Obsidian
---

# Cách cập nhật ghi chú lên Website

Bạn có thể viết bài trực tiếp trong Obsidian hoặc tạo file Markdown trong thư mục `content/`:

### 1. Viết bài mới
- Đặt file `.md` mới vào thư mục `content/` (ví dụ: `content/ghi-chu-moi.md`).
- Thêm tiêu đề ở đầu file (Frontmatter):
  ```markdown
  ---
  title: Tiêu đề bài viết
  ---
  ```

### 2. Tạo liên kết nội bộ
- Dùng cú pháp `[[Tên file]]` hoặc `[[Tên file|Tên hiển thị]]`. Quartz sẽ tự động chuyển thành link web và hỗ trợ popover preview.

### 3. Đồng bộ lên website
Mỗi khi có thay đổi, bạn chỉ cần commit và đẩy lên GitHub:
```bash
git add .
git commit -m "Thêm bài viết mới"
git push
```
Cloudflare Pages sẽ tự động kích hoạt tiến trình build và cập nhật website trong vòng 1 phút.

Quay lại: [[index|Trang chủ]]
