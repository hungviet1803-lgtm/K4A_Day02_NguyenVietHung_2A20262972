# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên:Nguyễn việt hùng 
- Mã học viên:2A20262972
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...):Developer tại công ty cung cấp phần mềm quản lý chung và các dịch vụ hỗ trợ, quản lý cho khách sạn.
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
-Phát triển và duy trì các chức năng phần mềm phục vụ quản lý và vận hành khách sạn.
-Code, kiểm thử và sửa lỗi các chức năng theo yêu cầu của dự án.
-Phân tích yêu cầu, xử lý các vấn đề phát sinh trong quá trình phát triển phần mềm.
-Làm việc với dữ liệu và hệ thống liên quan đến quản lý khách sạn, dịch vụ và thông tin khách hàng.
-Phối hợp với các thành viên trong nhóm để triển khai, cải thiện và bảo trì hệ thống.



## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 |    Viết nhiều đoạn code CRUD giống nhau/ Developer/ 5–10lần/tuần
| 2 |    Tìm và sửa bug mất nhiều thời gian/ Developer và tester/ 3–5 bug/tuần
| 3 |    Kiểm tra dữ liệu khách sạn thủ công/ Developer, 2–5lần/tuần
| 4 |    Tra cứu code và syntax nhiều lần/Developer/5–10 lần/tuần,
| 5 |    Viết test case thủ công/ Developer và tester/ 3–5chức năng/tuần
| 6 |    Khách hàng báo lỗi thiếu thông tin/ Developer và khách hàng/2–5 lần trao đổi/issue
| 7 |    Kiểm tra các bước trước khi deploy/Developer/2–5lần/tuần
| 8 |    Đọc code cũ để hiểu module/Developer/2–4 task/tuần,
| 9 | | | | |
| 10 | | | | |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi:Gợi ý các vấn đề có thể áp dụng AI trong công việc lập trình quản lý khách sạn
- Ý dùng được:Tìm bug,viết code,tạo test
- Ý bỏ vì không phải pain thật:Các vấn đề ít xảy ra hoặc không ảnh hưởng nhiều đến thời gian làm việc

**Self-check Phase 1:**
- [ X] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [ X] Dùng ít nhất 3/4 lăng kính
- [ X] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 |   Tìm và sửa bug/Thường gặp,ảnh hưởng tiến độ/Chưa đo thời gian
| 2 |   Viết test case/Lặp lại, dễ sai/Chưa đo hiệu quả AI
| 3 |   Tra cứu code/syntax/Xảy ra thường xuyên/Chưa đo số lần

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

– Tìm và sửa bug
Actor: Developer
Workflow: Nhận bug- kiểm tra log- tìm code -sửa- test
Bottleneck: Tìm nguyên nhân bug
Impact:  3–5 bug/tuần

-Viết test case
Actor: Developer
Workflow: Đọc yêu cầu -xác định case- viết test- chạy test- sửa lỗi
Bottleneck: Viết test case
Impact: 30–60 phút/chức năng

– Tra cứu code/syntax

Actor: Developer
Workflow: Gặp vấn đề -tìm kiếm- đọc tài liệu -thử code - hoàn thành
Bottleneck: Tìm thông tin phù hợp
Impact:5–10 lần/tuần


#### Problem Card #1 — [Tên problem]

```text
Problem 1 câu: Tìm nguyên nhân và sửa bug mất nhiều thời gian

Actor: Developer

Thời điểm / bối cảnh: Khi khách hàng báo lỗi

Current workflow 3-7 bước:
1. Nhận thông tin lỗi
2. Kiểm tra log
3. Tìm code liên quan
4. Xác định nguyên nhân
5. Sửa và test

Bottleneck:Tìm nguyên nhân bug

Impact:3–5 bug/tuần.

Success metric:Giảm thời gian tìm và sửa bug

Non-AI alternative: Cải thiện log và tài liệu code


AI hypothesis: AI hỗ trợ phân tích log và gợi ý nguyên nhân bug

Quick gut:Có khả năng áp dụng AI
[ x] No AI / process fix
[ ] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE —  60–120 phút

[1 Nhận bug: 5p] → [2 Kiểm tra log: 10p] → [3 Tìm code: 20p] → [4 Tìm nguyên nhân: 30–60p] <-- bottleneck

FUTURE STATE — 30–60 phút

[1 Nhận bug: 5px] → [2 AI phân tích log + code: 20p] → [3 Developer review: 5–35p] <-- human boundary

Fallback: nếu AI sai thì  Developer kiểm tra log và code thủ công
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — [Tên problem]

```text
Problem 1 câu:Viết test case thủ công mất thời gian và dễ bỏ sót

Actor:Developer

Thời điểm / bối cảnh:Khi hoàn thành chức năng mới

Current workflow 3-7 bước:
1.Đọc yêu cầu
2.Xác định trường hợp test
3.Viết test case
4.Chạy test
5.Sửa lỗi


Bottleneck:Xác định đầy đủ test case.

Impact:30–60p/chức năng.

Success metric:Giảm thời gian viết test và giảm test bị bỏ sót

Non-AI alternative:Dùng checklist test case

AI hypothesis:AI gợi ý test case và các trường hợp biên

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 30–60 phút

[1 Đọc yêu cầu: 10p] → [2 Xác định test case: 20p] → [3 Viết test + chạy test: 30p] <-- bottleneck

FUTURE STATE — 15–30 phút

[1 Đọc yêu cầu: 5p] → [2 AI gợi ý test case: 10p] → [3 Developer review: 10p] <-- human boundary

Fallback:Nếu AI thiếu hoặc sai test case thì Developer bổ sung thủ công
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — [Tên problem]

```text
Problem 1 câu:Tra cứu code và syntax nhiều lần khi lập trình

Actor:  Developer

Thời điểm / bối cảnh:Khi gặp vấn đề hoặc API chưa nhớ rõ

Current workflow 3-7 bước:
1. Gặp vấn đề
2. Tìm kiếm
3. Đọc tài liệu
4. Thử code
5. Hoàn thành

Bottleneck: Tìm thông tin phù hợp

Impact: 5–10 lần/tuần

Success metric: Giảm thời gian tra cứu

Non-AI alternative: Lưu lại tài liệu và code mẫu

AI hypothesis: AI giải thích syntax và đưa ví dụ phù hợp

Quick gut: Có thể áp dụng AI

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 10–20phút

[1 Gặp vấn đề: 2p] → [2 Tìm tài liệu: 8p] → [3 Đọc + thử code: 10p] <-- bottleneck

FUTURE STATE — 5–10p

[1 Mô tả vấn đề: 2p] → [2 AI gợi ý: 3p] → [3 Developer review + thử code: 5p] <-- human boundary

Fallback: Nếu AI trả lời sai thì kiểm tra documentation chính thức
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Problem Card 1: Tìm và sửa bug
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Quy trình tìm và sửa bug gồm nhiều bước bottleneck nằm ở việc tìm nguyên nhân
Mỗi bug mất khoảng 30–120p, 3–5bug/tuần,ảnh hưởng trực tiếp đến tiến độ
AI có thể hỗ trợ phân tích log và code để giảm thời gian xử lý
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
AI có thực sự xác định đúng nguyên nhân bug không
Cần giới hạn AI ở bước nào để tránh sửa code sai
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra:Chưa có số liệu đo chính xác
- Tôi sửa gì:Đo thời gian xử lý 5–10 bug thực tế

### Self-check nộp phần 01
- [X ] Có 5+ problems + top 3 Cards đủ field
- [X ] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [ X] Đã chọn 1 card pitch + câu hỏi challenge
