# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|-----|-----------|-------------|---------------------------------------------------------------|
| 1 | Đặng Thái Anh | 2A202602740 | Leader/facilitator, điều phối hội tụ và ghép bản cuối |
| 2 | Trần Ngọc Khánh | | Problem owner, cung cấp dữ liệu fanpage và validation |
| 3 | Phùng Đức Đăng | | Research, so sánh Rule/Workflow/Agent và rủi ro kỹ thuật |
| 4 | Đào Duy Hiếu | | Vẽ workflow trước/sau và chuẩn hóa báo cáo |
| 5 | Đỗ Thùy Dương | | Challenge, kiểm tra phương án thay thế và fallback |
| 6 | Hoàng Tuấn Thành | | Ghi log hội tụ, metric và theo dõi tiến độ |

**Candidate problem nhóm chọn (1 câu):**

Admin fanpage phải trả lời khoảng 30 tin nhắn mỗi ngày, thường xuyên mở bảng sản phẩm để tra cứu và soạn lại các câu trả lời lặp lại, làm tăng thời gian phản hồi và nguy cơ cung cấp thông tin thiếu nhất quán.

---

## Phase 3 — Group Convergence: từ 9-12 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Phùng Đức Đăng | Phải tạo lại boilerplate và cấu trúc lặp lại khi viết unit test. | Developer | Tạo mock, setup và cấu trúc test thủ công cho từng module. | Workflow rõ nhưng có thể giải phần lớn bằng template hoặc snippet. |
| 2 | Phùng Đức Đăng | Quy trình tạo branch, commit và merge giữa các thành viên không thống nhất. | Developer trong nhóm | Mỗi người đặt tên và thực hiện Git workflow khác nhau. | Pain thật nhưng ưu tiên process/rule trước AI. |
| 3 | Phùng Đức Đăng | Khi CI/CD thất bại phải đọc log dài để tìm nguyên nhân và hướng sửa. | Developer | Tìm dòng lỗi chính và liên hệ với thay đổi gây lỗi. | Phù hợp AI hỗ trợ tóm tắt nhưng chưa có baseline hoặc log mẫu. |
| 4 | Trần Ngọc Khánh | Fanpage nhận nhiều câu hỏi FAQ lặp lại nhưng admin vẫn phải tra bảng sản phẩm và trả lời thủ công. | Admin/CS fanpage | Mỗi chat phải mở bảng sản phẩm, tìm thông tin và soạn lại câu trả lời. | Evidence mạnh nhất: khoảng 30 chat/ngày, 60-180 giây/chat và 20% phải hỏi lại kho. |
| 5 | Trần Ngọc Khánh | Admin phải tự đọc và phân loại mức độ ưu tiên của từng tin nhắn. | Admin fanpage | Không có tiêu chí hoặc công cụ tự động gắn nhãn và ưu tiên chat. | Có evidence tốt, nhưng có thể ghép thành bước mở rộng sau FAQ. |
| 6 | Trần Ngọc Khánh | Admin dễ quên follow-up khách hàng vì phải nhớ thủ công nhiều hội thoại cũ. | Admin/CS fanpage | Không có nhắc việc theo ngữ cảnh; mở lại chat cũ mất thời gian. | Pain rõ nhưng cần tích hợp nền tảng và chính sách gửi tin. |
| 7 | Đào Duy Hiếu | Mỗi lần ứng tuyển phải sửa CV thủ công theo từng mô tả công việc. | Sinh viên/người tìm việc | Đọc JD, tìm keyword và chỉnh nhiều phần CV bằng tay. | Dữ liệu dễ lấy nhưng đề tài phổ biến và có rủi ro riêng tư. |
| 8 | Đào Duy Hiếu | Tổng hợp và định dạng báo cáo từ nhiều nguồn không thống nhất. | Nhân viên/nhóm trưởng | Thu thập, chuẩn hóa và trình bày dữ liệu thủ công. | Workflow rõ nhưng chưa có actor, file mẫu và baseline cụ thể. |
| 9 | Đào Duy Hiếu | Tìm việc trên nhiều nguồn tạo ra quá nhiều kết quả không phù hợp. | Sinh viên/người tìm việc | Phải lọc tin tuyển dụng phân tán và chất lượng không đồng đều. | Problem quá rộng; cần thu hẹp nguồn, ngành và tiêu chí. |
| 10 | Đặng Thái Anh | Hằng tuần phải lấy dữ liệu, làm sạch và chuẩn hóa trước khi cập nhật biểu đồ Power BI. | Nhân viên kỹ thuật | Ghép file, sửa schema, timestamp, đơn vị và dữ liệu bất thường thủ công. | Workflow thực tế và đo được nhưng chưa có baseline và dữ liệu mẫu được xác nhận. |
| 11 | Đặng Thái Anh | Hằng ngày phải tổng hợp thông tin từ email, Zalo và Facebook. | Nhân viên kỹ thuật/quản lý dự án | Chuyển đổi giữa nhiều kênh, loại trùng và xác định việc cần làm. | Pain hằng ngày nhưng phạm vi tích hợp, quyền truy cập và bảo mật phức tạp. |
| 12 | Đặng Thái Anh | Dịch tài liệu sang ngôn ngữ khác nhưng vẫn phải giữ nguyên cấu trúc file. | Nhân viên kỹ thuật/người làm hồ sơ | Chèn lại nội dung và sửa lỗi thuật ngữ, font, bảng biểu hoặc bố cục. | Có prototype thực tế và dễ demo; cần giới hạn định dạng file và đo baseline. |
| 13 | Đỗ Thùy Dương | Khi CI/CD lỗi cần tóm tắt nguyên nhân và gửi thông báo dễ hiểu qua chat. | Developer/DevOps | Đọc log dài, xác định nguyên nhân và viết lại thông báo thủ công. | Trùng nhiều với candidate #3; nên gom cùng cluster. |
| 14 | Đỗ Thùy Dương | Lịch học, lịch thi và lịch cá nhân phân tán nên dễ quên. | Sinh viên/người dùng cá nhân | Phải tự tổng hợp và nhập từng lịch vào công cụ nhắc việc. | Có thể giải bằng calendar/rule; AI chỉ cần cho bước trích xuất lịch. |
| 15 | Đỗ Thùy Dương | Developer mất thời gian đọc lỗi và tìm hướng sửa trong dự án. | Developer | Xác định ngữ cảnh lỗi và chọn thay đổi mã nguồn an toàn. | Phạm vi quá rộng và rủi ro cao nếu AI tự sửa. |
| 16 | Đỗ Thùy Dương | Developer phải tự nghĩ nhiều trường hợp kiểm thử và viết test thủ công. | Developer | Xác định edge case, tạo dữ liệu test và đảm bảo coverage. | Gần candidate #1; AI có thể gợi ý nhưng người dùng vẫn phải review. |
| 17 | Hoàng Tuấn Thành | Công việc cá nhân và công việc nhóm có nhiều deadline nhưng người dùng phải tự theo dõi và nhắc lại. | Cá nhân/thành viên nhóm | Deadline nằm rải rác; phải tự nhập, kiểm tra và nhắc từng việc. | Pain rõ nhưng rule/calendar có thể đủ; cần chứng minh phần nào thực sự cần AI. |

### 3.2. Gom trùng / cluster (gom 9-12 ý thành 3-4 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A — Hỗ trợ phát triển phần mềm | #1, #2, #3, #13, #15, #16 | Tự động hóa thao tác lặp lại trong code, test, Git và CI/CD. | Nhiều bài có thể giải bằng rule/template; bài tự sửa code có rủi ro cao. |
| B — Vận hành fanpage/CS | #4, #5, #6 | Đọc, phân loại, tra cứu và phản hồi lượng chat lớn. | Có actor, workflow, log và metric cụ thể nhất. |
| C — Tài liệu và tổng hợp thông tin | #7, #8, #9, #11, #12 | Thu thập, lọc, viết lại hoặc chuyển đổi nội dung từ nhiều nguồn. | Cần thu hẹp phạm vi, định dạng và quyền truy cập. |
| D — Dữ liệu vận hành và quản lý thời gian | #10, #14, #17 | Chuẩn hóa dữ liệu hoặc chuyển thông tin thành báo cáo/lịch nhắc. | SmartPV có giá trị domain; lịch/deadline nên ưu tiên rule trước AI. |

### 3.3. Shortlist (giữ 2-3 bài trả lời được 7 câu hỏi worksheet)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| Trợ lý tạo câu trả lời FAQ cho fanpage | Có số liệu thực tế; actor và bottleneck rõ; có thể pilot bằng chat lịch sử và bảng sản phẩm mà chưa cần tích hợp API. | Cần xác nhận câu trả lời chuẩn, dữ liệu sản phẩm có cập nhật không và admin nào chịu trách nhiệm review. |
| Làm sạch dữ liệu vận hành để cập nhật Power BI | Công việc thật, lặp lại hằng tuần; workflow đầu vào/đầu ra rõ; impact có thể đo bằng thời gian và lỗi dữ liệu. | Chưa có baseline, file mẫu và xác nhận cách lấy dữ liệu tự động; ý tưởng đang trộn dữ liệu có cấu trúc với OCR tài liệu. |
| Dịch tài liệu nhưng giữ nguyên cấu trúc file | Đã có trải nghiệm dùng tool kết hợp AI; dễ tạo demo trước/sau; có thể đo thời gian, lỗi thuật ngữ và lỗi bố cục. | Phạm vi thay đổi theo DOCX/PPTX/XLSX/PDF; chữ trong ảnh và bố cục phức tạp có thể không được giữ nguyên. |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Trợ lý tạo câu trả lời FAQ cho fanpage | 5 | 5 | 5 | 5 | 5 | 5 | 4 | 34 |
| Làm sạch dữ liệu vận hành để cập nhật Power BI | 5 | 5 | 3 | 4 | 4 | 5 | 5 | 31 |
| Dịch tài liệu nhưng giữ nguyên cấu trúc file | 5 | 5 | 3 | 4 | 5 | 5 | 4 | 31 |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
Admin fanpage phải trả lời khoảng 30 tin nhắn mỗi ngày, thường xuyên mở bảng sản phẩm để tra cứu và soạn lại các câu trả lời lặp lại, làm tăng thời gian phản hồi và nguy cơ cung cấp thông tin thiếu nhất quán.
```

**Vì sao chọn (4-5 câu):**

```text
Nhóm chọn bài toán FAQ fanpage vì actor, workflow và bottleneck đều quan sát được trực tiếp. Log hiện có cho thấy khoảng 30 chat mỗi ngày, mỗi chat mất 60-180 giây và admin phải mở bảng sản phẩm ít nhất một lần; khoảng 20% câu hỏi còn phải hỏi lại kho. Nhóm có thể pilot nhỏ bằng 30-50 chat lịch sử và bảng sản phẩm, không cần cho AI tự gửi tin. Kết quả có thể đo bằng thời gian xử lý, tỷ lệ draft được chấp nhận và số lỗi thông tin. So với các candidate khác, bài này có evidence và khả năng chạy thử trong lab tốt nhất.
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
Không chọn SmartPV/Power BI vì nhóm chưa có baseline thời gian, file mẫu và xác nhận quyền truy cập dữ liệu; phần làm sạch có cấu trúc cũng có thể được giải phần lớn bằng Power Query hoặc rule. Không chọn bài dịch giữ nguyên cấu trúc vì phạm vi thay đổi mạnh theo định dạng file và chưa có số liệu về số file, thời gian hoặc lỗi hiện tại. Hai bài này vẫn được giữ làm phương án dự phòng nếu validation fanpage không xác nhận pain.
```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text
Chưa ghi nhận disagreement chính thức trong sheet. Nhóm tạm chốt bằng bảng score, ưu tiên evidence và pilot nhỏ thay vì chọn bài chỉ vì nghe mới hoặc phức tạp; quyết định sẽ được xác nhận lại sau quick validation với admin fanpage.
```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Interview | | | | |
| Survey / poll | | | | |
| Log / ticket / review (nếu có) | | | | |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text

```

Bằng chứng đính kèm (nếu có): `02-group-problem-statement-survey.png`, `...-interview-notes.md`

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text

```

> Lưu ý: không dùng số liệu AI đưa nếu không verify được link chính thức. Ghi rõ giả định chưa chắc.

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.png/pdf/md`

```text
[1 ...: __' - ai làm] → [2 ...: __'] → [3 ...: __'] → [4 ... bottleneck: __'] → ...
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |

**Bottleneck chính (2-3 câu):**

```text

```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, boundary ở đâu, fallback khi AI sai.

```text
[1 ...: __' - máy] → [2 AI ...: __'] → [3 ... review: __' - boundary] → [4 ... gửi]

Fallback: ...
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Tổng thời gian | | | |
| Số bước | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Risk mới | | | |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | |
| **Workflow** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** | |
| **Boundary** | |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ:
- Tôi sửa gì:

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [ ] Thấp (có đúng/sai rõ) / [ ] Cao (nhiều cách trả lời vẫn OK) — Vì sao:
- Độ phức tạp: [ ] Thấp (1-2 bước) / [ ] Cao (3+ bước/nguồn, phụ thuộc nhau) — Vì sao:

**Bài toán nhóm nằm ở ô nào:**

```text

```

**Vì sao (2-3 câu):**

```text

```

### 6.1. So sánh Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. Rule có giải được 70-80% case không?
2. Các bước có đi thẳng một đường không hay phải rẽ nhánh?
3. Có thật sự cần Agent tự lập kế hoạch + gọi tool không?
4. Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu?
5. Có hạ được từ Agent → Workflow → Rule không?

**Mức chọn:**

```text
[Rule / Workflow / Agent]
```

**Vì sao chọn (3-4 câu):**

```text

```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text

```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | |
| **Workflow** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** | |
| **Boundary** (làm / không làm) | |
| **AI intervention point** (can thiệp sau bước nào, trước bước nào) | |
| **Mức chọn** (Rule / Workflow / Agent + 1 câu vì sao) | |
| **Rủi ro & người thật kiểm tra** (rủi ro lớn nhất + ai kiểm tra bằng cách nào) | |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | | |
| Baseline + metric đo được chưa? | | |
| Data/input đủ dùng chưa? | | |
| AI sai, hậu quả chấp nhận được không? | | |
| Có người review/owner không? | | |
| Có cách non-AI đơn giản hơn không? | | |

**Decision:**

```text
[Go / Not Yet / No-Go]
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text

```

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text

```

**Nếu Not Yet — cần validate gì trước:**

```text

```

**Nếu No-Go — làm gì thay AI:**

```text

```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text

```

---

### Self-check nộp phần 02 (nhóm)
- [ ] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score)
- [ ] Có validation (quote thật) + research (link kiểm được)
- [ ] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [ ] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [ ] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do
