# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Đào Ngọc Bình Thiên
- Mã học viên: 2A202602814
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): intern AI Engineer
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem): Tổng hợp weekly report, Viết dailystandup mỗi ngày, Tra cứu tài liệu, tìm hiểu thuật ngữ công ty.

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 |Mất thời gian |Người mới mất thời gian tìm tài liệu và hiểu thuật ngữ nội bộ |Intern, Nhân viên mới, Mentor |2 tiếng/ngày |
| 2 |Pain từ người khác |Mentor khó theo dõi tiến độ của Intern |Mentor, Intern |3 lần meeting/tuần |
| 3 |Tốn thời gian |Chuẩn bị weekly report mỗi tuần |Intern |1 lần/tuần |
| 4 |Lặp lại |Viết standup update mỗi ngày |Intern |1 lần/ngày |
| 5 |Tốn thời gian |Viết meeting notes sau mỗi buổi họp |Intern |30 phút/buổi |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |
| 9 | | | | |
| 10 | | | | |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi:
- Ý dùng được:
- Ý bỏ vì không phải pain thật:

**Self-check Phase 1:**
- [ ] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [ ] Dùng ít nhất 3/4 lăng kính
- [ ] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 |Người mới mất thời gian tìm tài liệu và hiểu thuật ngữ nội bộ |Giúp người mới onboarding nhanh hơn, giảm các câu hỏi lặp lại cho mentor. Tài liệu nội bộ chính xác, có nguồn, giải thích thuật ngữ cụ thể |Người mới, intern có thực sự muốn hỏi AI hay không. Tính bảo mật của dữ liệu nội bộ công ty |
| 2 |Mentor khó theo dõi tiền độ của Intern |Mentor sẽ thấy rõ tiến độ của intern, có thể hỗ trợ mà không cần hỏi thủ công mỗi ngày |Mentor thực sự thiếu thông tin hay thiếu thời gian đọc. Những đánh giá này có thực sự là đánh giá công tâm |
| 3 |Chuẩn bị weekly report |Xuất hiện đều đặn, lặp đi lặp lại, người mới khó làm quen |Mentor có thật sự cần một format chung cho các thành viên intern không |

### 2.2. Problem Cards chi tiết

---

#### Problem Card #1 — Tìm tài liệu và thuật ngữ nội bộ

```text
Problem 1 câu: Người mới mất nhiều thời gian tìm đúng tài liệu và hiểu thuật ngữ nội bộ.

Actor: Intern, nhân viên mới và mentor.

Thời điểm / bối cảnh: Khi bắt đầu một task mới hoặc gặp thuật ngữ chưa biết.

Current workflow 3-7 bước:
1. Đọc yêu cầu công việc.
2. Tìm tài liệu trong các thư mục hoặc chat.
3. Hỏi mentor khi chưa hiểu thuật ngữ.
4. Đọc lại tài liệu và thực hiện task.

Bottleneck: Tài liệu phân tán, khó biết tài liệu nào là đúng và mới nhất.

Impact: Người mới mất khoảng 2 giờ/ngày; mentor phải trả lời các câu hỏi lặp lại.

Success metric: Giảm thời gian tìm hiểu xuống dưới 1 giờ/ngày và giảm số câu hỏi lặp lại cho mentor.

Non-AI alternative: Gom tài liệu vào một nơi và làm danh mục thuật ngữ chung.

AI hypothesis: AI tìm kiếm theo ngữ nghĩa, trả lời ngắn gọn và dẫn link tới tài liệu nguồn.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — khoảng 120 phút

[Đọc task: 10'] → [Tìm tài liệu: 60'] → [Hỏi mentor: 20'] → [Hiểu và làm task: 30']  <-- bottleneck

FUTURE STATE — khoảng 60 phút

[Đọc task: 10'] → [Hỏi AI và xem nguồn: 20'] → [Tự kiểm tra/mentor review: 30']  <-- human boundary

Fallback: Nếu AI không chắc hoặc không có nguồn, hỏi mentor và cập nhật tài liệu chung.
```

---

#### Problem Card #2 — Mentor khó theo dõi tiến độ intern

```text
Problem 1 câu: Mentor khó nắm được intern đang làm gì và đang vướng ở đâu.

Actor: Mentor và intern.

Thời điểm / bối cảnh: Trong các buổi meeting, khoảng 3 lần/tuần.

Current workflow 3-7 bước:
1. Intern tự ghi lại việc đã làm.
2. Đến meeting, intern báo cáo miệng.
3. Mentor hỏi thêm về tiến độ và khó khăn.
4. Hai bên thống nhất việc tiếp theo.

Bottleneck: Thông tin không được cập nhật liên tục, mentor phải hỏi lại từ đầu.

Impact: Meeting dài hơn và mentor khó hỗ trợ đúng lúc.

Success metric: Mentor xem được tiến độ trước meeting; giảm thời gian hỏi cập nhật trong meeting.

Non-AI alternative: Dùng bảng Kanban chung, cập nhật trạng thái task mỗi ngày.

AI hypothesis: AI tóm tắt daily standup thành tiến độ, việc đang làm và blocker cho mentor xem.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — mỗi buổi meeting

[Intern nhớ lại việc đã làm] → [Báo cáo miệng] → [Mentor hỏi thêm]  <-- bottleneck

FUTURE STATE

[Intern cập nhật ngắn mỗi ngày] → [AI tóm tắt] → [Mentor xem và trao đổi blocker]  <-- human boundary

Fallback: Nếu tóm tắt thiếu, mentor xem bản standup gốc và hỏi trực tiếp intern.
```

---

#### Problem Card #3 — Chuẩn bị weekly report

```text
Problem 1 câu: Intern mất thời gian tổng hợp công việc trong tuần để viết weekly report.

Actor: Intern và mentor.

Thời điểm / bối cảnh: Cuối mỗi tuần.

Current workflow 3-7 bước:
1. Xem lại daily standup, task và meeting notes.
2. Chọn các việc quan trọng.
3. Viết kết quả, khó khăn và kế hoạch tuần sau.
4. Chỉnh sửa theo format rồi gửi mentor.

Bottleneck: Phải đọc lại thông tin ở nhiều nơi và tự sắp xếp thành báo cáo.

Impact: Mỗi tuần đều lặp lại, làm chậm thời gian hoàn thành báo cáo.

Success metric: Hoàn thành bản nháp trong 15 phút và ít phải sửa format.

Non-AI alternative: Dùng mẫu weekly report cố định, cập nhật dần trong tuần.

AI hypothesis: AI tổng hợp daily standup và task thành bản nháp theo mẫu; intern kiểm tra trước khi gửi.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — khoảng 30 phút

[Xem lại nhiều nguồn: 15'] → [Tổng hợp nội dung: 10'] → [Chỉnh format: 5']  <-- bottleneck

FUTURE STATE — khoảng 15 phút

[Đưa daily standup/task vào AI: 5'] → [AI tạo bản nháp: 2'] → [Intern kiểm tra và sửa: 8']  <-- human boundary

Fallback: Nếu bản nháp sai, dùng mẫu report cố định và tự chỉnh từ thông tin gốc.
```

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Problem Card #1 — Tìm tài liệu và thuật ngữ nội bộ.
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Người mới hiện mất khoảng 2 giờ/ngày để tìm tài liệu và hiểu thuật ngữ nội bộ.
Giải pháp là một AI tìm kiếm có nguồn, giúp trả lời nhanh nhưng vẫn để người dùng kiểm tra tài liệu gốc.
Việc này giúp onboarding nhanh hơn và giảm câu hỏi lặp lại cho mentor.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
Làm sao đảm bảo AI chỉ dùng tài liệu được phép và không trả lời sai về thông tin nội bộ?
Nếu tài liệu chưa đầy đủ hoặc đã cũ thì ai sẽ chịu trách nhiệm cập nhật?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra: Dữ liệu nội bộ có thể cũ, thiếu hoặc cần bảo mật.
- Tôi sửa gì: Chỉ dùng tài liệu đã được duyệt, luôn hiển thị nguồn và có mentor kiểm tra khi cần.

### Self-check nộp phần 01
- [ ] Có 5+ problems + top 3 Cards đủ field
- [ ] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [ ] Đã chọn 1 card pitch + câu hỏi challenge
