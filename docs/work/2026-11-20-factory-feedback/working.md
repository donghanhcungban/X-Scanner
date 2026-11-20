# Đồng bộ vòng phản hồi cho X-Scanner

Work ID: 2026-11-20-factory-feedback

Giữ bản nền X-Templates 3.29.0 và guard hiện có. Cổng repo giới hạn mỗi tệp 1 MiB: hai tệp nguồn ở bản 3.34.0 hiện vượt giới hạn. Backport từ `www-donghanhcungban-org/X-Templates@3a1cd5471cb1f634656c62369559c4a489a58dcc` hai thay đổi độc lập: `loop verify` nhóm các lệnh tương đương một lần; `test-shard-plan` giữ thứ tự trọng số giảm dần trong mỗi shard.

Hướng dẫn `/factory` cho công cụ lập trình dùng Flutter hot reload, test theo tệp, rồi trình MVP bằng cổng APK hiện có. Không thay binary, dữ liệu scan hay cấu hình phát hành. Hoàn tác bằng revert commit tích hợp. Cổng nghiệm thu là Framework and Android app gate trong PR #85.
