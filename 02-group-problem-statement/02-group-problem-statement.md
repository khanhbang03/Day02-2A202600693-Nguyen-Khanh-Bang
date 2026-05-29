# 02 — Group Problem Statement

## Goal

This is the group deliverable. The team should work together on one final document covering:

- Convergence log / meeting notes
- Validation and research
- Problem Statement
- Rule / Workflow / Agent discussion
- Final decision
- Before/after workflows

## 1. Group convergence log

- **Session 1 (May 28, 2026, 14:00-14:30):** Each member shared top 3 candidate problems. Bang presented weekly update synthesis, decision search, and rubric check. Two other members shared similar issues in status reporting and review follow-up.
- **Session 2 (May 28, 2026, 15:00-15:20):** Group clustered candidates into three themes: information synthesis, retrieval of past decisions, and submission accuracy. We scored each candidate and discussed feasibility in the 4-hour lab.
- **Session 3 (May 28, 2026, 15:50-16:10):** Final shortlist and validation plan. Group agreed đi sâu vào một problem có workflow rõ, evidence thật và phù hợp AI hỗ trợ.

### Candidates shared by each member

- Bang: weekly status update, tìm decision cũ trong Discord, so khớp rubic nộp bài.
- Member 2: tổng hợp feedback review, viết meeting note, kiểm tra checklist nộp sản phẩm.
- Member 3: search tài liệu cũ, xác nhận task, tổng hợp data từ CRM/Slack.

### How the group clustered

| Cluster | Candidates | Common pattern |
|---|---|---|
| Information synthesis | Weekly update, meeting note, feedback summary | Gom nhiều nguồn rồi viết lại thành bản tóm tắt rõ ràng |
| Retrieval | Find decision in Discord, recall requirement, search old docs | Tìm lại evidence/requirement nhanh khi cần |
| Submission certainty | Rubric check, review checklist, file completeness | Giảm sai sót trước khi nộp hoặc gửi |

### Shortlist and scoring

| Candidate | Actor rõ | Workflow rõ | Evidence | Feasibility | AI fit | Total |
|---|---|---|---|---|---|---|
| Weekly update synthesis | 5 | 5 | 4 | 5 | 5 | 24 |
| Retrieval of past decision | 4 | 4 | 4 | 4 | 4 | 20 |
| Rubric / submission check | 4 | 4 | 3 | 5 | 3 | 19 |

Group chose: **Weekly update synthesis**.

## 2. Validation / research

### Validation

- Interviewed 4 peers in class and project group.
- 3/4 reported rằng họ thường mất 45-90 phút để tổng hợp nội dung từ nhiều nguồn mỗi tuần.
- Một bạn cho biết phần khó nhất là viết narrative ngắn gọn, không phải thu thập dữ liệu.
- Có một peer phản bác: team của họ dùng template cứng và đã giảm được một phần thời gian, nhưng vẫn mất effort ở bước viết cho nội dung mới.

### Research

| Source | What they solve | Insight | Gap |
|---|---|---|---|
| Notion AI / Google Docs AI | Summarize notes, rewrite text | Good for tóm tắt, nhưng cần input sạch | Không tự động gom nhiều nguồn khác nhau |
| Slack AI summary | Tóm tắt conversation | Giúp lấy ý chính từ chat | Không xử lý được số liệu từ Jira/Figma/Google Sheets |
| Weekly report template | Giảm format work | Hữu ích để chuẩn hóa | Vẫn phải tự viết phần insight và action |

### Research notes

- AI rất phù hợp khi dữ liệu đầu vào đã được cấu trúc sơ bộ.
- Xây hoàn toàn agent tự động có rủi ro hallucination nếu đầu vào quá lộn xộn.
- Workflow hợp lý là dùng rule để gom dữ liệu, sau đó AI hỗ trợ draft narrative, và con người review.

## 3. Problem Statement

**Actor:** Junior product / lab member hoặc project member cần nộp weekly status update.

**Problem:** Khi phải tổng hợp tiến độ và ghi nhận kết quả từ nhiều nguồn như Slack, Google Docs, Figma và Google Sheets, người làm mất nhiều thời gian viết narrative rõ ràng.

**Context:** Cuối mỗi tuần hoặc trước buổi review nội bộ, người chịu trách nhiệm phải gửi cập nhật ngắn gọn cho nhóm và giảng viên.

**Bottleneck:** Việc biến dữ liệu thô và note rời rạc thành nội dung tóm tắt đủ rõ cho người đọc.

**Impact:** Mất 60-90 phút mỗi tuần, dẫn đến giảm thời gian thực thi công việc, dễ bỏ sót thông tin quan trọng và giảm chất lượng báo cáo.

**Success metric:** Giảm tổng thời gian soạn status update xuống dưới 30 phút mà vẫn giữ được độ chính xác và rõ ràng. Fallback: không có AI support, người làm vẫn hoàn thành trong 45 phút.

**Boundary / scope:**
- Bao gồm: tổng hợp nội dung từ nguồn text và note nội bộ, đề xuất cấu trúc status update, draft narrative.
- Không bao gồm: tự động kéo dữ liệu từ hệ thống bảo mật chưa có quyền truy cập; gửi email thay người dùng; thay thế hoàn toàn người review.

## 4. Rule / Workflow / Agent

### No AI alternative

- Dùng template weekly update và checklist.
- Mất nhiều công sức hơn ở bước viết narrative.
- Ưu điểm: ít rủi ro hơn, dễ thực hiện.

### Rule / automation alternative

- Dùng script hoặc form để gom dữ liệu từ các nguồn sẵn có.
- Giảm thời gian thu thập nhưng vẫn cần người viết phần insight.
- Ưu điểm: đáng làm nếu dữ liệu có cấu trúc.

### AI / agent alternative

- AI dùng để tóm tắt nội dung và đề xuất câu văn, không thay thế quyết định người dùng.
- Hợp lý nếu input được gom, lọc và đặt trong bối cảnh cụ thể.
- Giảm bottleneck ở bước viết narrative.

### Why final choice

Group quyết định chọn **Workflow + AI assistance**.
- Rule / template không giải quyết đủ phần viết ý chính.
- Agent toàn phần quá rủi ro khi dữ liệu chưa ổn định.
- Workflow hợp lý nhất là: gom dữ liệu → AI draft → human review.

### Human boundary and review

- Người dùng vẫn kiểm tra lại nội dung; AI chỉ là gợi ý draft.
- Nếu AI output sai hoặc thiếu context, người dùng bỏ draft và tự viết.
- Con người chịu trách nhiệm quyết định phần nào nên gửi.

## 5. Final decision

- **Decision:** Go with AI-assisted workflow.
- **Why:** Problem có workflow rõ, pain thật, dữ liệu có thể gom được, và phần AI hỗ trợ là writing / summarization, không phải quyết định.
- **Risks:** AI hallucination, output thiếu chính xác, dữ liệu đầu vào không đủ rõ.
- **Fallback plan:** Nếu AI không cho kết quả tốt, dùng template manual và vẫn giữ workflow gom dữ liệu thô.

## 6. Workflow before / after

### Current workflow

```text
CURRENT STATE — 70-90 phút
[1 Thu thập nguồn thủ công: 20'] → [2 Lọc thông tin: 15'] → [3 Viết narrative: 25'] → [4 Format + review: 15'] → [5 Gửi: 5']
```

### Future workflow

```text
FUTURE STATE — 25-30 phút
[1 Gom dữ liệu cơ bản: 10'] → [2 AI đề xuất nội dung chính: 5'] → [3 Human review + chỉnh sửa: 15'] → [4 Gửi: 3']
```

### Notes

- Bottleneck hiện tại: viết narrative từ dữ liệu thô.
- AI được đặt ở bước đề xuất nội dung, không phải quyết định cuối cùng.
- Human review là checkpoint bắt buộc trước khi gửi.

## 7. Supporting files

- Nếu có thể, nhóm sẽ thêm `02-group-problem-statement-workflow.pdf` để minh họa flowchart.
- Nếu cần, ghi lại note research vào `02-group-problem-statement-research-notes.md`.
