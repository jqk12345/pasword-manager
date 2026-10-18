# Quy ước làm việc

## Nhánh
- Không push thẳng lên `main`. Mọi thay đổi đi qua pull request.
- Mỗi issue một nhánh, tạo từ `main`: `feature/<số-issue>-<tên-ngắn>`, ví dụ `feature/12-room-schema`.
- Sửa lỗi: `fix/<số-issue>-<tên-ngắn>`. Tài liệu: `docs/<số-issue>-<tên-ngắn>`.

## Commit
Theo [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: thêm màn hình danh sách mật khẩu
fix: xóa clipboard sau 30 giây
docs: thêm mô hình STRIDE
test: unit test cho mã hóa AES-GCM
chore: cấu hình CI
```

## Pull request
- Điền đủ PR template, ghi `Closes #<số-issue>` để issue tự đóng khi merge.
- Cần CI xanh và ít nhất 1 approval.
- PR sửa `crypto`, `auth`, `keystore`, `autofill` cần trưởng nhóm duyệt (CODEOWNERS tự gán).
- Merge bằng **Squash and merge**, xóa nhánh sau khi merge.

## Bảo mật
- Repo này là public: không commit mật khẩu, key, keystore file, ảnh hay số giấy tờ thật.
- Chỉ dùng dữ liệu giả trong test, ảnh chụp màn hình và demo.
- Log không được chứa mật khẩu, khóa, số giấy tờ hay dữ liệu đã giải mã.

## Phiên bản
- Cuối mỗi giai đoạn gắn tag `v0.<số-giai-đoạn>.0` và cập nhật `CHANGELOG.md`.

## Họp
- Họp nhóm hằng tuần: <!-- điền thứ, giờ, địa điểm -->
- Họp giảng viên hướng dẫn: theo lịch giảng viên.
