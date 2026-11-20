---
name: factory
description: Nối vòng phát triển X-Scanner từ MVP chạy thử, hoàn thiện đến tối ưu bằng các lệnh Flutter và cổng hiện có.
---

# /factory — X-Scanner

1. Đọc `AGENTS.md`, `CLAUDE.md`, `PROJECT.md`, `PROGRESS.md` và work ID hiện tại. Chạy `python3 .xtemplates/scripts/xt.py stage status --json`. Với repo đang vận hành mà chưa có sổ stage, dùng quy trình duyệt/adopt của dự án trước khi ghi trạng thái.
2. **MVP.** Chọn một luồng scan hoặc export với tiêu chí có thể kiểm. Khi sửa ứng dụng, vào `apps/mobile`, chạy `flutter run` trên thiết bị hoặc emulator rồi nhấn `r` để hot reload. Chạy `flutter test test/app_test.dart` hoặc tệp test cụ thể cho luồng vừa sửa. Trước khi trình, chạy `bash scripts/dev-task.sh gate` từ gốc repo; trình cách thử và chờ phản hồi của người duyệt.
3. **Hoàn thiện.** Sau khi MVP được duyệt, hoàn tất tiêu chí, kiểm ca lỗi và rà soát cả luồng. Tập hợp việc độc lập vào một PR theo work ID và điền mẫu PR của repo.
4. **Tối ưu.** Sau khi hoàn thiện, đo trên cùng bộ tài liệu thử và thiết bị, sửa rồi đo lại. Giữ quy trình riêng của X-Scanner cho kiểm thử thiết bị, quyền riêng tư, ký và phát hành.
