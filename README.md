# LƯU Ý

Quy định chung.

---

## I. 🚦 Git Workflow

1. **Tuyệt đối không commit trực tiếp lên:**`main`

   * Luôn tạo nhánh mới để phát triển: `git checkout -b feature/ten-chuc-nang`

2. **Cập nhật nhánh chính trước khi phát triển:**

   ```bash
   git checkout main
   git pull origin main
   git checkout feature/ten-chuc-nang
   git merge main
   ```

3. **Commit message rõ ràng, nhất quán và có ý nghĩa cụ thể.**

   ```
   feat: thêm giao diện giỏ hàng
   fix: sửa lỗi responsive header
   ```

4. **Đẩy code thường xuyên** để tránh xung đột và mất dữ liệu.

5. **Resolve conflict tại local trước khi merge lên main.**

---

## II. 🌿 Branch Naming Convention

| Loại      | Tiền tố     | Ví dụ                    |
| --------- | ----------- | ------------------------ |
| Tính năng | `feature/`  | `feature/login-page`     |
| Sửa lỗi   | `bugfix/`   | `bugfix/fix-cart-update` |
| Refactor  | `refactor/` | `refactor/navbar-ui`     |
| Hotfix    | `hotfix/`   | `hotfix/crash-on-login`  |

---

## III. ✅ Commit Message Convention

```bash
<type>: mô tả ngắn gọn
```

| Type     | Ý nghĩa                                  |
| -------- | ---------------------------------------- |
| feat     | Thêm tính năng mới                       |
| fix      | Sửa lỗi                                  |
| refactor | Cải tiến code không làm thay đổi hành vi |
| style    | Thay đổi style/format code               |
| chore    | Việc lặt vặt (build, config, deps)       |
| docs     | Thay đổi liên quan tài liệu              |
| test     | Thêm hoặc cập nhật test                  |

---

> Nếu có thay đổi, toàn nhóm phải đồng thuận và cập nhật file README.md.
