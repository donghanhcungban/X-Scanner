# Công việc: Mở mã MIT, thêm mục ủng hộ và hỗ trợ triển khai

- Work ID: 2026-11-16-open-source-donate
- Yêu cầu / outcome: chủ repo quyết định mở mã mọi repo cá nhân theo MIT (`Copyright (c) 2026 seeker19110`), thêm mục ủng hộ (VietQR Techcombank) và dịch vụ hỗ trợ triển khai (TP. HCM hoặc online). Đóng RK-005 (chưa chọn giấy phép sản phẩm).
- Trạng thái: In review
- Chủ trì / writer: phiên chính; chủ repo duyệt và merge.
- Mức rủi ro / số PR: S, một PR chỉ tài liệu/giấy phép, không đổi app, quyền Android, gate, CI hay dependency.
- Scope / non-goal: `LICENSE`, `NOTICE`, `.github/FUNDING.yml`, `docs/assets/donate-vietqr-techcombank.png`, README (mục ủng hộ, mục giấy phép), `docs/RISKS.md` RK-005, hai câu về license trong `PROJECT.md`, `CHANGELOG.md`, hồ sơ này. Non-goal: phát hành app, ký số, chính sách nhãn hiệu.
- Spec / goal / issue: quyết định của chủ repo 2026-11-16 (không có issue).
- Nhánh / base SHA / thời điểm reconcile: `docs/open-source-donate` @ `95418bc` · 2026-11-16T03:06:58Z

## Kế hoạch và phân công

Một PR, phiên chính viết. Không subagent.

## Quyết định và bằng chứng

- Giấy phép: MIT, văn bản chuẩn giống `third_party/X-Templates.LICENSE`.
- Quét bí mật toàn lịch sử: `gitleaks git --redact` 175 commit → 0 phát hiện. `.mcp.json` trong lịch sử chỉ có URL MCP công khai, không khoá.
- Rà bản quyền: icon launcher Android/iOS (`apps/mobile/android/app/src/main/res/mipmap-*/ic_launcher.png`, `apps/mobile/ios/Runner/Assets.xcassets/AppIcon.appiconset/*`) là icon mặc định của `flutter create` — logo Flutter, nhãn hiệu của Google; cần thay bằng icon riêng trước phát hành (chủ repo quyết). Ảnh/PDF trong `docs/ops/evidence/` là ảnh chụp emulator với trang mẫu tổng hợp; `third_party/` giữ license MIT của khung. Không thấy asset/mã bên thứ ba khác — ghi ở `NOTICE`.

## Lần thử / blocker

Không có.

## Bàn giao / bước tiếp theo

Chờ chủ repo review và merge PR; sau merge đổi tên hồ sơ thành `done.md`.

## Nghiệm thu cuối (chỉ điền khi đủ bằng chứng)

Chưa nghiệm thu.
