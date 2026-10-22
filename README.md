# IT Portfolio — Lê Ngọc Nam

Portfolio tĩnh cho hồ sơ IT (backend / software engineer). Nội dung tiếng Việt.

## Xem local

Mở `index.html` hoặc chạy server tĩnh từ thư mục này.

## Cloudflare Pages

Site không cần build. `wrangler.toml` chỉ khai báo `pages_build_output_dir = "."`.

Trong **Workers & Pages → project → Settings → Builds**:

- Framework preset: **None**
- Build command: để trống
- Build output directory: `.`
- Branch: `main`

Build command đang là `npx wrangler deploy` thì xóa. Đó là lệnh Workers. Pages thấy `pages_build_output_dir` nên cảnh báo, rồi fail vì không có Worker script.

Nếu log dừng ở `Cloning repository`, Cloudflare chưa đọc được GitHub repo. Cấp quyền repo cho GitHub App **Cloudflare Pages**, rồi push `main`.

## Chỉnh nội dung

Sửa tên, email, stack, dự án và kinh nghiệm trong `index.html`.
