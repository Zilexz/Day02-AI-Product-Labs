# 01 — Individual Problem Scan

> Bài cá nhân Day 02 Lab. Bối cảnh: sinh viên năm cuối ngành Khoa học Máy tính, đang làm đồ án tốt nghiệp và phải viết báo cáo tiến độ hằng tuần, đồng thời tham gia khóa đào tạo AI thực chiến (sáng học lý thuyết, chiều làm bài lab).

---

## Scan rộng — 10 problems

Tôi scan 10 problems từ trải nghiệm thật, vượt mức tối thiểu 5.

| # | Lăng kính | Problem quan sát được | Ai đang đau? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Lặp lại | Mỗi tuần phải viết báo cáo tiến độ đồ án gửi GVHD: tuần này làm gì, kẹt gì, tuần sau làm gì | Tôi (SV làm đồ án) | ~60 phút/tuần, làm đều mỗi tuần suốt kỳ đồ án |
| 2 | Lặp lại | Mỗi chiều sau lab AI phải viết reflection + chuẩn bị bài nộp theo cùng một cấu trúc | Tôi và các bạn cùng khóa | ~25 phút/buổi, lặp lại hằng ngày |
| 3 | Tốn thời gian | Đọc và tóm tắt paper/tài liệu tiếng Anh cho phần cơ sở lý thuyết của đồ án | Tôi (SV làm đồ án) | 40-60 phút/paper, cần đọc 15-20 paper |
| 4 | Tốn thời gian | Tổng hợp lại lý thuyết buổi sáng để chuẩn bị làm lab buổi chiều | Tôi và các bạn cùng khóa | 20-30 phút/ngày, sợ bỏ sót ý quan trọng |
| 5 | AI có thể tốt hơn | Tìm lại đoạn code cũ hoặc lý do mình đã chọn một cách làm khi debug đồ án | Tôi (SV làm đồ án) | 10-15 phút/lần tìm, vài lần/tuần |
| 6 | AI có thể tốt hơn | Ghi lại cấu hình và kết quả mỗi lần train model (learning rate, accuracy, loss...) để so sánh | Tôi (SV làm đồ án) | Train 5-10 lần/ngày, hay quên ghi nên phải train lại |
| 7 | Pain từ người khác | Feedback của GVHD rải rác qua email, Zalo, và lời nói trong buổi gặp, khó tổng hợp lại | Tôi, và GVHD phải nhắc lại | Hay quên 1-2 ý feedback giữa các buổi gặp |
| 8 | Tốn thời gian | Format trích dẫn và danh mục tài liệu tham khảo đúng chuẩn IEEE của trường | Tôi (SV làm đồ án) | 30-45 phút mỗi lần chỉnh, dễ sai format |
| 9 | Lặp lại | Theo dõi cùng lúc 3 luồng việc: đồ án, lý thuyết sáng, lab chiều — dễ rơi task | Tôi và các bạn cùng khóa | 1-2 task bị rơi/tuần vì không có chỗ tổng hợp |
| 10 | AI có thể tốt hơn | Tìm lại câu trả lời/thông tin cũ (quy trình nộp, deadline, cấu trúc repo) trong Discord khóa học vì search kém | Tôi và các bạn cùng khóa | 10-15 phút/lần tìm, cùng câu hỏi lặp lại 2-3 lần/tuần |

**Vì sao phần scan này đủ mạnh:**

- Scan rộng (10 problems) trước khi hội tụ, vẫn cụ thể chứ không chung chung.
- Có đủ 4 lăng kính: lặp lại, tốn thời gian, AI có thể tốt hơn, pain từ người khác.
- Mỗi problem có actor thật và dấu hiệu đo được (thời gian, tần suất).
- Không bắt đầu bằng "xây chatbot" hay "làm agent toàn năng" — bắt đầu từ workflow thật.

---

## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Báo cáo tiến độ đồ án hằng tuần (#1) | Workflow rõ, lặp lại đều, có metric thời gian tốt, dễ vẽ before/after | "Báo cáo đủ tốt" để GVHD hiểu đo thế nào |
| 2 | Đọc & tóm tắt paper cho cơ sở lý thuyết (#3) | Tốn thời gian lớn, AI thực sự có thể hỗ trợ đọc/tóm tắt | Chất lượng tóm tắt khó đo, rủi ro AI hiểu sai paper |
| 3 | Tìm câu trả lời cũ trong Discord (#10) | Nhiều người gặp, AI/search có thể hỗ trợ | Data access và privacy có thể phức tạp |

---

## Problem Card #1 — Báo cáo tiến độ đồ án hằng tuần

**Problem 1 câu:**
Mỗi tuần tôi mất khoảng 60 phút viết báo cáo tiến độ đồ án gửi GVHD, trong đó bước nhớ lại và sắp xếp những gì đã làm cả tuần tốn nhất và dễ viết sót hoặc lan man.

**Actor:**
Sinh viên năm cuối đang làm đồ án tốt nghiệp, chịu trách nhiệm gửi báo cáo tiến độ hằng tuần cho giảng viên hướng dẫn.

**Thời điểm / bối cảnh:**
Cuối mỗi tuần, sau một tuần vừa làm đồ án vừa học khóa AI, trước buổi gặp/nộp báo cáo cho GVHD.

**Current workflow:**

```text
1. Mở lại Git log / các file code đã sửa trong tuần
2. Lục lại note rời, tab trình duyệt, tin nhắn để nhớ cả tuần đã làm gì
3. Nhớ lại những chỗ bị kẹt và đã thử gì trong tuần
4. Viết báo cáo: tuần này làm gì, kết quả, kẹt gì, kế hoạch tuần sau
5. Đọc lại, chỉnh câu chữ cho mạch lạc
6. Gửi cho GVHD qua email/Zalo
```

**Bottleneck:**
Bước 2-4 — nhớ lại và sắp xếp công việc rải rác cả tuần thành một báo cáo mạch lạc mất khoảng 40 phút, vì thông tin nằm rải ở nhiều chỗ và việc của cả tuần dễ nhớ sót.

**Impact:**
Khoảng 60 phút/tuần, làm đều mỗi tuần suốt kỳ đồ án (vài tháng). Báo cáo viết vội thường thiếu chi tiết hoặc lan man, khiến GVHD khó nắm tiến độ và phải hỏi lại trong buổi gặp.

**Success metric:**
Giảm thời gian viết báo cáo từ ~60 phút xuống dưới 25 phút/tuần; không tăng số lần GVHD phải hỏi lại vì báo cáo thiếu thông tin.

**Non-AI alternative:**
Một template báo cáo cố định + thói quen ghi note ngắn mỗi ngày trong tuần. Cách này giảm được bước nhớ lại nhưng chưa giải quyết bước biến note rời thành đoạn văn mạch lạc.

**AI hypothesis:**
AI nhận note rời / Git log cả tuần và draft một báo cáo có cấu trúc (đã làm / kết quả / kẹt / kế hoạch). Tôi đọc lại, sửa và gửi — AI không tự gửi.

**Quick gut:**
`[ ] No AI  [ ] Rule  [x] Workflow  [ ] Agent  [ ] Chưa biết`

### Workflow trước/sau

```text
CURRENT STATE — 6 bước, ~60 phút/tuần

[1 Mở Git log / file đã sửa cả tuần: 6']
→ [2 Lục note rời, tab, tin nhắn cả tuần: 12']
→ [3 Nhớ lại các chỗ kẹt + đã thử gì: 10']
→ [4 Viết báo cáo mạch lạc: 18']        <-- bottleneck
→ [5 Đọc lại, chỉnh câu chữ: 8']
→ [6 Gửi GVHD qua email/Zalo: 6']

FUTURE STATE — 5 bước, ~23 phút/tuần

[1 Ghi note ngắn mỗi ngày khi làm: ~0' thêm]      -- thói quen
→ [2 Dán note cả tuần + Git log vào prompt: 3']
→ [3 AI draft báo cáo tuần có cấu trúc: 1']        -- AI hỗ trợ
→ [4 Tôi review + sửa nội dung: 15']               <-- human boundary
→ [5 Tôi gửi GVHD: 4']

Tiết kiệm ~37 phút/tuần.
Fallback: AI draft sai/nhạt hoặc bịa việc tôi chưa làm → tôi tự viết lại từ note thật.
```

---

## Problem Card #2 — Đọc & tóm tắt paper cho cơ sở lý thuyết

**Problem 1 câu:**
Khi viết phần cơ sở lý thuyết của đồ án, tôi mất 2-3 giờ để đọc, ghi chú và so sánh mỗi paper tiếng Anh, và phải làm với 15-20 paper nên rất chậm, ghi chú không nhất quán và dễ quên paper nào nói gì.

**Actor:**
Sinh viên năm cuối đang viết chương cơ sở lý thuyết / tổng quan nghiên cứu cho đồ án tốt nghiệp.

**Thời điểm / bối cảnh:**
Giai đoạn đầu và giữa đồ án, khi cần đọc nhiều paper để xây dựng phần lý thuyết và so sánh các hướng nghiên cứu.

**Current workflow:**

```text
1. Tìm paper trên arxiv/Google (thủ công)
2. Đọc toàn bộ paper PDF 15-30 trang
3. Ghi chú rời rạc vào note, không có cấu trúc chuẩn
4. Tự so sánh với các paper cũ đã đọc
5. Tổng kết vào bản nháp chương cơ sở lý thuyết
```

**Bottleneck:**
Bước 2-4 — đọc toàn bộ paper tiếng Anh dày 15-30 trang (60-90 phút) rồi tự so sánh với paper cũ (thêm 30-40 phút); ghi chú không có cấu trúc chuẩn nên khó tra lại.

**Impact:**
2-3 giờ/paper × 15-20 paper = rất nhiều ngày công. Ghi chú không nhất quán dễ quên paper nào nói gì, phải mở lại paper cũ nhiều lần khi viết.

**Success metric:**
Giảm thời gian xử lý mỗi paper từ ~2-3 giờ xuống còn ~20 phút (tiết kiệm ~2 giờ/paper); mỗi paper có một bản tóm tắt chuẩn template (Problem / Method / Result) kèm so sánh với paper trước để tra nhanh khi viết.

**Non-AI alternative:**
Một bảng note chuẩn theo template để ghi tóm tắt thủ công, giúp ghi chú nhất quán hơn nhưng không giảm được thời gian đọc.

**AI hypothesis:**
AI nhận link/PDF paper, tóm tắt theo template Problem/Method/Result và tự so sánh với database notes của các paper trước. Tôi vẫn phải đọc lại bản gốc ở những chỗ quan trọng để verify, vì rủi ro hiểu sai paper rất cao.

**Quick gut:**
`[ ] No AI  [ ] Rule  [x] Workflow  [ ] Agent  [ ] Chưa biết`

### Workflow trước/sau

```text
CURRENT STATE — 5 bước, 2-3 giờ/paper

[1 Tìm paper trên arxiv/Google: 20-30']
→ [2 Đọc toàn bộ paper PDF 15-30 trang: 60-90']    <-- bottleneck
→ [3 Ghi chú rời rạc vào note: không cấu trúc chuẩn]
→ [4 Tự so sánh với paper cũ: +30-40']
→ [5 Tổng kết: ghi chú không nhất quán]

FUTURE STATE — 5 bước, ~20 phút/paper

[1 Input: link / file PDF paper]                   -- người dùng cung cấp
→ [2 AI tóm tắt theo template: Problem/Method/Result] -- AI hỗ trợ
→ [3 AI so sánh paper trước: tự động từ database notes] -- AI hỗ trợ
→ [4 Người dùng review + sửa: 10-15']              <-- human boundary
→ [5 Tổng kết: chuẩn template, có so sánh]

Tiết kiệm ~2 giờ/paper.
Fallback: AI tóm tắt sai trọng tâm hoặc bịa kết quả → quay lại đọc bản gốc đầy đủ.
```

---

## Problem Card #3 — Tìm câu trả lời cũ trong Discord

**Problem 1 câu:**
Khi cần biết lại quy trình nộp bài, deadline hay cấu trúc repo, tôi và các bạn phải cuộn và search trong Discord khóa học mất nhiều phút; search kém nên hay không thấy và phải hỏi lại, làm cùng câu hỏi lặp đi lặp lại.

**Actor:**
Học viên khóa AI thực chiến cần tra cứu lại thông tin / hỏi-đáp cũ trong server Discord của khóa.

**Thời điểm / bối cảnh:**
Mỗi khi làm bài lab buổi chiều hoặc chuẩn bị nộp, cần tra lại thông tin từng được hỏi-đáp trước đó trong Discord.

**Current workflow:**

```text
1. Nhớ mơ hồ là thông tin này từng được nói đâu đó trong Discord
2. Search keyword / cuộn qua nhiều channel
3. Đọc nhiều message rời để tìm đúng câu trả lời
4. Nếu không thấy thì đăng câu hỏi lại trong channel
5. Chờ bạn khác hoặc trợ giảng trả lời
```

**Bottleneck:**
Bước 2-3 — search Discord theo keyword cho kết quả kém và rời rạc, phải đọc nhiều thread mới ra; nếu vẫn không thấy thì phải hỏi lại và chờ, làm gián đoạn việc đang làm.

**Impact:**
10-15 phút/lần tìm, vài lần/tuần, cho nhiều học viên trong khóa. Cùng câu hỏi lặp lại 2-3 lần/tuần làm nhiễu channel và tốn thời gian của trợ giảng phải trả lời lại.

**Success metric:**
Giảm thời gian tìm một câu trả lời cũ từ ~12 phút xuống dưới 3 phút; giảm số câu hỏi lặp lại trong channel (đo bằng số lần cùng một câu hỏi xuất hiện lại trong 2 tuần).

**Non-AI alternative:**
Một kênh `#faq` được ghim + tài liệu Q&A tổng hợp cập nhật thủ công. Giải quyết tốt các câu hỏi phổ biến nhưng không bao phủ được thông tin rải rác trong lịch sử chat.

**AI hypothesis:**
Một trợ lý search/RAG chạy trên lịch sử Discord (hoặc bộ tài liệu khóa học) để trả lời câu hỏi cũ bằng ngôn ngữ tự nhiên và trích nguồn message gốc. Rủi ro: cần quyền truy cập lịch sử chat và xử lý dữ liệu cá nhân của học viên, nên data access và privacy có thể phức tạp.

**Quick gut:**
`[ ] No AI  [ ] Rule  [x] Workflow  [ ] Agent  [ ] Chưa biết`

### Workflow trước/sau

```text
CURRENT STATE — 4 bước, ~12 phút/lần tìm

[1 Nhớ mơ hồ thông tin từng có trong Discord: 1']
→ [2 Search keyword / cuộn nhiều channel: 5']      <-- bottleneck
→ [3 Đọc nhiều message rời để tìm đúng câu: 4']
→ [4 Không thấy → hỏi lại + chờ trả lời: 2'+ (chờ thêm)]

FUTURE STATE — 3 bước, dưới 3 phút/lần tìm

[1 Hỏi trợ lý bằng câu tự nhiên: 0.5']
→ [2 AI search Discord/tài liệu + trích link nguồn: 1'] -- AI hỗ trợ
→ [3 Tôi mở link nguồn để verify: 1']              <-- human boundary

Tiết kiệm ~9 phút/lần tìm và bớt câu hỏi lặp.
Fallback: AI không tìm thấy hoặc trả lời lỗi thời → search thủ công hoặc hỏi trợ giảng.
Phạm vi: cần được phép truy cập lịch sử Discord + xử lý dữ liệu cá nhân;
nếu không, thu hẹp về search trên bộ tài liệu/FAQ chính thức của khóa.
```

---

## Chọn card muốn pitch nhất

**Card tôi muốn pitch nhất:**

```text
Problem Card #1 — Báo cáo tiến độ đồ án hằng tuần.
```

**Vì sao:**

```text
- Workflow rõ ràng và tôi đang sống với nó mỗi tuần nên hiểu rất sâu.
- Có baseline thời gian cụ thể (~60 phút/tuần) để đo before/after.
- Lặp lại đều đặn nên cải thiện nhỏ cũng tích lũy thành giá trị lớn.
- Có thể so sánh được No AI (template) / Workflow (AI draft + người review),
  và có ranh giới con người rõ (tôi review và gửi, AI không tự gửi).
- Đây cũng là pain chung của nhiều bạn cùng khóa, dễ validate nhanh.
```

**Câu hỏi tôi muốn nhóm challenge:**

```text
1. "Báo cáo đủ tốt" cho GVHD nên đo bằng gì ngoài thời gian — số lần bị hỏi lại?
   độ hài lòng? — và đo thế nào cho khách quan?
2. Liệu chỉ cần một template tốt + thói quen ghi note đã giải quyết phần lớn vấn đề
   chưa, hay AI thực sự thêm giá trị ở bước viết narrative?
3. Rủi ro AI bịa ra việc tôi chưa làm trong báo cáo gửi GVHD lớn cỡ nào,
   và làm sao kiểm soát?
```

---

## Ghi chú dùng AI ở phần cá nhân này

Tôi tự scan và tự viết các Problem Card trước. Nếu dùng AI ở phần này, tôi chỉ dùng để:

- Gợi ý thêm góc nhìn problem theo 4 lăng kính sau khi đã tự scan — rồi tự bỏ ý nào không phải pain thật của mình.
- Đóng vai PM hoài nghi để phản biện Problem Card (chỉ ra điểm yếu, không khen), giúp tôi siết lại metric và bottleneck.

Những ý sẽ ghi vào reflection: AI gợi ý được gì dùng được, ý nào tôi bỏ vì không có workflow thật, và chỗ nào tôi tự sửa lại bằng nhận định của mình.

---

*01 — Individual Problem Scan · Day 02 Lab*
