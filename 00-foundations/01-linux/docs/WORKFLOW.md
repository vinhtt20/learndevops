# 📋 Quy trình soạn tài liệu Linux (Claude Multi-Agent Pipeline)

Tài liệu được sản xuất qua một dây chuyền nhiều "chuyên gia" (mỗi chuyên gia là một agent độc lập).
Mục tiêu: **độ chính xác tuyệt đối** + trình bày chuẩn LaTeX + xuất PDF sạch.

## Đối tượng độc giả
- Người Việt **chưa có kiến thức kỹ thuật** (non-tech).
- Dùng **laptop macOS**.
- Cần giải thích từ con số 0, ví dụ gần gũi, không thuật ngữ khó hiểu nếu chưa định nghĩa.

## Các giai đoạn (pipeline)

| # | Vai trò chuyên gia | Việc làm | Đầu ra |
|---|--------------------|----------|--------|
| 1 | **Chuyên gia Linux (Author)** | Viết nội dung chương, bám sát đối tượng macOS/non-tech | Bản thảo nội dung |
| 2 | **Hội đồng review kỹ thuật (3 người, độc lập)** | Soi từng câu, bắt lỗi sai kiến thức, đối chiếu thực tế macOS | Danh sách lỗi/chỉnh sửa |
| 3 | **Author (revise)** | Sửa theo toàn bộ góp ý → nội dung chính xác tuyệt đối | Nội dung cuối |
| 4 | **Chuyên gia LaTeX** | Chuyển nội dung sang LaTeX (XeLaTeX, hỗ trợ tiếng Việt) | mã `.tex` |
| 5 | **Chuyên gia audit LaTeX** | Soi mã: biên dịch được không, typography, lỗi cú pháp | `.tex` đã sửa |
| 6 | **Biên dịch PDF** (Claude/Bash) | Chạy `xelatex`, sửa lỗi biên dịch nếu có | `linux-tai-lieu.pdf` |
| 7 | **Kiểm tra PDF** | Đếm trang, trích text, kiểm font/dấu tiếng Việt, đối chiếu nội dung | Báo cáo PASS/FAIL |

## Nguyên tắc chất lượng
- **Adversarial review:** reviewer được yêu cầu *cố tìm lỗi*, mặc định nghi ngờ.
- **Chính xác tuyệt đối:** mọi lệnh/khái niệm phải đúng trên macOS/Linux thực tế. Nghi ngờ → loại bỏ.
- **Không placeholder:** không để "TODO", không bịa lệnh.
- **Tiếng Việt chuẩn:** dấu hiển thị đúng trong PDF (kiểm tra bằng pdftotext).

## Cấu trúc thư mục
- `docs/src/`     — mã nguồn LaTeX (`main.tex`)
- `docs/build/`   — PDF đã biên dịch
- `docs/content/` — bản thảo nội dung trung gian (markdown)
- `docs/review/`  — báo cáo review / audit

## Cách chạy lại
Pipeline được điều phối bằng công cụ Workflow của Claude. Mỗi lần chạy sẽ tái lập đủ 7 giai đoạn.

## 🎓 Chuẩn sư phạm bắt buộc
Mọi chương tuân theo `PEDAGOGY.md`: thực hành ngay + ghi nhớ chủ động (active recall, flashcards, ôn ngắt quãng) + hộp "Góc Senior" để hướng tới trình độ senior DevOps.
