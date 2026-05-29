# Day 02 Lab - Tìm đúng bài toán cho AI

Thông tin cần thay:

- Mã học viên: `2A202600680`
- Họ tên: `Nguyễn Đức Hiếu`
- Nhóm: `4`
- Case nhóm chọn: Tự động hóa báo cáo tiến độ định kỳ từ hoạt động đã làm

## Cấu trúc bài nộp

| Phần | File |
|---|---|
| 01 - Individual Problem Scan | [individual-problem-scan.md](01-individual-problem-scan/individual-problem-scan.md) |
| 02 - Group Problem Statement | [group-problem-statement.md](02-group-problem-statement/group-problem-statement.md) |
| 02 - Future Workflow Diagram | [future_workflow_v1.svg](02-group-problem-statement/future_workflow_v1.svg) |
| 03 - Individual Reflection | [individual-reflection.md](03-individual-reflection/individual-reflection.md) |

## Tóm tắt bài làm

Cá nhân đã scan 10 problems từ trải nghiệm thực tế làm đồ án tốt nghiệp và khóa học AI. Top 3 problem được chọn để pitch là:

1. Sinh viên năm cuối mất ~60 phút/tuần viết báo cáo tiến độ đồ án gửi GVHD thủ công.
2. Sinh viên mất 2-3 giờ đọc và tóm tắt mỗi paper tiếng Anh cho phần cơ sở lý thuyết.
3. Học viên mất 10-15 phút/lần tìm lại câu trả lời cũ trong Discord khóa học vì search kém.

Nhóm chọn candidate problem số 1 vì actor rõ, workflow tuyến tính vẽ được, bottleneck cụ thể (nhớ lại cả tuần + viết phần khó khăn/lý giải trễ), metric thời gian đo được (60-80 phút/tuần) và có thể so sánh No AI / Rule / Workflow / Agent.

## Quyết định cuối

Mức chọn: `Workflow`.

Decision: `Go với scope nhỏ`.

Lý do: Bài toán có workflow rõ, AI chỉ hỗ trợ đúng một bước (draft 4 mục: Đã làm / % milestone / Khó khăn-Giải pháp / Kế hoạch) sau khi sinh viên gom note và commit log. Sinh viên vẫn review và tự nộp, AI không tự nộp, không tự bịa việc chưa làm. Pilot 2 tuần dữ liệu thật, rollback về template nếu tỉ lệ phải viết lại vượt 40%.
