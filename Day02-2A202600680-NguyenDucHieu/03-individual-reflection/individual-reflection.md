# 03 — Individual Reflection

> Vai trò trong nhóm: **Research & Validation Lead** (phụ trách Phase 4). Candidate nhóm chọn: *Báo cáo tiến độ định kỳ từ hoạt động đã làm*.

## Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| Scan cá nhân | Đưa ra 10 problems với baseline thời gian cụ thể cho từng bài (phút/lần, lần/tuần) | Mỗi candidate có dấu hiệu đo được trước khi nhóm chọn — tránh chọn vì cảm giác |
| Pitch Problem Card | Pitch báo cáo tiến độ định kỳ với baseline ~60 phút/tuần và 3 câu hỏi challenge rõ | Nhóm có điểm xuất phát đo được để so before/after |
| Challenge bài của bạn khác | Hỏi về cách đo chất lượng tóm tắt ở bài paper, và quyền truy cập lịch sử chat ở bài Discord search | Nhóm thấy rõ rủi ro metric khó đo và data access/privacy — loại trừ được 2 candidate yếu hơn |
| Quick validation | Đối chiếu baseline 60 phút/tuần với 4 thành viên + phỏng vấn 6 bạn cùng khóa + mini poll 10 người trong lớp | Xác nhận pain là thật, thu hẹp problem từ "viết hộ toàn bộ" thành "draft phần đã làm + khó khăn" |
| Research tool landscape | Tìm và đánh giá Geekbot, DailyBot, Gitmore, Kestra, n8n, ai-commit-report-generator-cli | Nhóm không nhảy ngay vào build từ đầu; xác nhận pattern Workflow đã có trên thị trường |
| Phân tích khoảng trống | So sánh tool đã có với bài toán của nhóm — chỉ ra Geekbot/DailyBot giải bước thu thập, chưa giải bước narrative | Nhóm không bị nhầm "tool có sẵn" với "giải hết vấn đề"; thấy rõ AI nằm đúng chỗ nào |
| Validate pilot | Đề xuất đo pilot bằng 3 chỉ số: phút bỏ ra, tỉ lệ phải viết lại, số lỗi % sai | Có cách đo cụ thể trước khi chạy, không chỉ dựa vào cảm giác sau khi dùng |
| Rollback condition | Đề xuất ngưỡng thoát: viết lại > 40% trong 2 tuần liên tiếp → lùi về template | Nhóm có exit rõ ràng thay vì commit mù vào một hướng |

## Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Gợi ý thêm góc nhìn sau khi tự scan | Nhớ thêm bài tìm quyết định cũ và meeting summary | Một số ý quá rộng kiểu "trợ lý research toàn năng" | Bỏ ý không có baseline thật |
| Challenge | Nhờ AI liệt kê rủi ro tiềm ẩn của từng candidate | Chỉ ra metric "nhanh hơn" là mơ hồ; data access là rào cản thật với Discord | AI hay kết luận "khó nhưng vẫn làm được" mà không lượng hóa khó cỡ nào | Tự thêm cột "Rủi ro / điều chưa rõ" vào shortlist để nhóm nhìn rõ hơn |
| Validation | Nhờ AI thiết kế câu hỏi phỏng vấn nhanh | Gợi ý hỏi về bước nào tốn công nhất thay vì hỏi chung "mất bao lâu" | AI đề xuất validation quá formal (survey dài, N lớn) so với thời gian lab | Hạ về 6 người interview + 10 người poll, đủ để xác nhận chiều hướng |
| Research | Nhờ AI gợi ý danh mục tool cần tìm | Biết nhìn vào Geekbot, Gitmore, Kestra, n8n, CLI open source | Có claim về tiết kiệm thời gian không kèm nguồn | Chỉ giữ link tool chính thức kiểm tra được; ghi rõ khoảng trống từng tool |
| Phân tích khoảng trống | Nhờ AI so sánh tool đã có với bài toán nhóm | Giúp phân loại rõ 2 hướng: question-based vs activity-based | AI có xu hướng kết luận "dùng Gitmore là đủ" quá sớm | Tự phân tích thêm: Gitmore chỉ thấy phần trong git, không thấy việc ngoài code |
| Pilot design | Nhờ AI gợi ý cách đo pilot | Gợi ý đo thời gian + tỉ lệ viết lại + lỗi % sai | AI đề xuất auto-pull tích hợp Jira/Git quá sớm cho pilot đầu tiên | Hạ scope về paste input thủ công + review để chạy được trong lab |

## Reflection

Qua lab này, tôi học được rằng validation không phải là bước làm cho có sau khi đã chọn xong, mà là thứ quyết định nhóm có đang giải đúng problem không. Lúc đầu khi nhóm pitch báo cáo tiến độ, con số 60 phút/tuần đến từ trải nghiệm của tôi — hợp lý nhưng dễ thiên kiến. Khi tôi đi phỏng vấn nhanh 6 bạn cùng khóa và poll thêm 10 người, nhóm mới thấy pain thật không nằm ở "gõ chữ", mà ở đoạn nhớ lại cả tuần và viết phần "khó khăn / lý giải trễ tiến độ" — chi tiết đó thay đổi cả hướng giải.

Là người phụ trách research và validation, đóng góp lớn nhất của tôi là giữ cho nhóm không build trong chân không. Khi tôi đưa ra Geekbot, Gitmore, Kestra, n8n vào bàn, nhóm thấy ngay rằng hướng Workflow này đã có người làm và còn khoảng trống ở đúng chỗ nhóm muốn vào: phần narrative "khó khăn / kế hoạch" mà tool hiện có chưa giải được. Đó là lý do nhóm tự tin chọn Workflow thay vì lo lắng "liệu có bị tool cũ lấn không".

AI hữu ích khi giúp tôi mở rộng danh mục tool cần tìm và thiết kế câu hỏi phỏng vấn, nhưng nếu để AI kết luận thay thì nó hay bỏ qua rủi ro thật: Gitmore chỉ thấy commit, không thấy việc ngoài code; Geekbot thu thập được nhưng không draft được narrative. Tôi phải tự phân tích khoảng trống từng tool và viết lại cột "khoảng trống / rủi ro" bằng nhận định của mình.

Nếu làm lại, tôi sẽ validate baseline 60-80 phút/tuần với nhiều bạn cùng khóa hơn trước khi nhóm chốt metric — đặc biệt là hỏi những người ít commit code hoặc ghi note tệ hơn, vì đó là nhóm AI sẽ khó hỗ trợ nhất. Tôi cũng sẽ challenge nhóm sớm hơn: nếu chỉ dùng template + commit log có mô tả, giải được bao nhiêu phần trăm pain — trước khi đưa AI vào.

## Nếu làm lại:

```text
Tôi sẽ validate baseline 60-80 phút/tuần với nhiều bạn cùng khóa hơn,
đặc biệt hỏi người ít commit code hoặc ghi note tệ — vì đó là nhóm AI
sẽ khó hỗ trợ nhất và cũng là nơi rủi ro "AI bịa việc chưa làm" cao nhất.

*03 — Individual Reflection · Day 02 Lab*
```
