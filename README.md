# Lộ trình triển khai Base × DALYTECH

Gồm: `index.html` (trang), `middleware.js` (hỏi mật khẩu), `package.json`, `vercel.json`.

## Triển khai lên Vercel
1. Tạo repo GitHub **Private**, upload các file này ngay ở gốc (không bọc thêm thư mục).
2. Vercel → Add New → Project → Import repo. Framework: Other, Root `./`, để trống Build/Output.
3. Environment Variables: thêm `SITE_PASSWORD` (tự gõ mật khẩu) TRƯỚC khi Deploy; nếu thêm sau thì Redeploy.

## Cập nhật nội dung
- Cách 1 (nhanh): mở trang với đuôi `?edit=1` (vd `https://ten-mien/?edit=1`), bấm vào chữ có viền cam để sửa, tick "Đã tổ chức", dán link Drive vào ô link, rồi bấm **Tải HTML** (hoặc Sao chép HTML) và thay file `index.html` trong repo. Vercel tự deploy lại.
- Cách 2: sửa trực tiếp khối dữ liệu `<script id="data" type="application/json">` đầu file `index.html`.
- Thử trạng thái theo ngày: thêm `?today=2026-11-20`.
