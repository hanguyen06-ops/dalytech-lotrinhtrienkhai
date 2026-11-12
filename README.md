# Lộ trình triển khai Base × DALYTECH (trang public, không mật khẩu)

Cấu trúc (các file nằm ngay ở gốc repo, không bọc thêm thư mục):

```
public/index.html   <- trang lộ trình
vercel.json
README.md
```

## Triển khai
1. Tạo repo GitHub, upload đúng cấu trúc trên (giữ nguyên thư mục `public`).
2. Vercel -> Add New -> Project -> Import repo. Framework: **Other**. Root Directory `./`. Để trống Build Command; Output Directory đã có sẵn trong vercel.json (`public`).
3. Deploy. Ai có link đều mở được, không cần mật khẩu. Trang có thẻ noindex nên Google không đưa lên kết quả tìm kiếm.

## Cập nhật nội dung
- Mở `https://ten-mien/?edit=1`, bấm vào chữ có viền cam để sửa, tick "Đã tổ chức", dán link Drive vào ô link, bấm **Tải HTML**, rồi thay file `public/index.html` trong repo. Vercel tự deploy lại. (Sửa trên trang chỉ lưu trong trình duyệt của người sửa, không làm đổi trang thật cho đến khi thay file.)
- Hoặc sửa thẳng khối `<script id="data" type="application/json">` ở đầu `public/index.html`.
- Xem thử theo ngày khác: thêm `?today=2026-11-20`.
