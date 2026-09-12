# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên:
- Mã học viên:
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Nhân viên kỹ thuật trong lĩnh vực điện mặt trời
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
  - Tải datasheet và dữ liệu vận hành từ Huawei SmartPV, làm sạch dữ liệu và cập nhật Power BI.
  - Kiểm tra, tổng hợp thông tin công việc từ email, Zalo và Facebook.
  - Theo dõi tin tức về điện mặt trời, công nghệ, thiết bị, thị trường và quy định liên quan.
  - Dịch datasheet, báo cáo và tài liệu kỹ thuật sang ngôn ngữ khác nhưng giữ nguyên cấu trúc file.
  - Kiểm tra cảnh báo trên Huawei SmartPV, tra cứu nguyên nhân và theo dõi quá trình xử lý.

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Lặp lại / Tốn thời gian / AI có thể tốt hơn | Hằng tuần phải tải datasheet, kéo dữ liệu từ Huawei SmartPV, làm sạch và chuẩn hóa số liệu rồi đưa vào các biểu đồ tải trên Power BI; quy trình thủ công dễ xảy ra sai sót. | Nhân viên kỹ thuật và người sử dụng báo cáo Power BI | Thực hiện hằng tuần; cần đo số giờ xử lý, số file/site và số lỗi dữ liệu phải sửa mỗi tuần. |
| 2 | Lặp lại / Tốn thời gian / Pain từ người khác | Hằng ngày phải kiểm tra email, Zalo và Facebook để tìm thông báo, yêu cầu hoặc cập nhật liên quan đến công việc; thông tin phân tán nên dễ bị bỏ sót, trùng lặp hoặc phản hồi chậm. | Nhân viên kỹ thuật, quản lý dự án và người gửi yêu cầu | Thực hiện hằng ngày trên ít nhất 3 kênh; cần đo thời gian kiểm tra và số thông tin bị bỏ sót hoặc phản hồi chậm. |
| 3 | Lặp lại / Tốn thời gian / AI có thể tốt hơn | Phải thường xuyên tìm kiếm và cập nhật tin tức về ngành điện mặt trời, công nghệ, thiết bị, thị trường và quy định từ nhiều nguồn khác nhau. | Nhân viên kỹ thuật và quản lý | Thực hiện hằng ngày hoặc hằng tuần; cần đo số nguồn phải đọc, thời gian đọc và số tin thực sự liên quan. |
| 4 | Tốn thời gian / AI có thể tốt hơn | Phải dịch datasheet, báo cáo hoặc tài liệu kỹ thuật sang ngôn ngữ khác trên cùng file nhưng vẫn giữ nguyên bố cục, bảng biểu, hình ảnh và định dạng. | Nhân viên kỹ thuật và người tiếp nhận tài liệu | Cần đo số file hoặc số trang mỗi tháng, thời gian dịch, số lỗi thuật ngữ và số lỗi định dạng sau khi dịch. |
| 5 | Lặp lại / Tốn thời gian / Pain từ người khác | Hằng ngày phải kiểm tra nhiều cảnh báo trên Huawei SmartPV, xác định mức độ quan trọng, tra cứu nguyên nhân và theo dõi quá trình xử lý; cảnh báo trùng có thể làm bỏ sót sự cố nghiêm trọng. | Nhân viên kỹ thuật vận hành và chủ sở hữu hệ thống | Thực hiện hằng ngày; cần đo số cảnh báo, thời gian phân loại, số cảnh báo trùng và số sự cố bị xử lý chậm. |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |
| 9 | | | | |
| 10 | | | | |

### Giả thuyết giải pháp AI cho 5 vấn đề

1. **Làm sạch dữ liệu và cập nhật Power BI:** Xây dựng workflow tự động OCR/Parse các file chứng chỉ hoặc datasheet, trích xuất thông số kỹ thuật, làm sạch dữ liệu và xuất theo định dạng chuẩn để cập nhật trực tiếp vào Power BI.
2. **Tổng hợp thông tin từ nhiều kênh:** Xây dựng AI Agent tổng hợp thông tin từ các kênh được cấp quyền, loại bỏ nội dung trùng, phân loại theo dự án và mức độ khẩn cấp, sau đó tạo bản tóm tắt công việc hằng ngày.
3. **Theo dõi và cập nhật tin tức:** Xây dựng workflow theo dõi các nguồn tin cố định, tự động lọc theo chủ đề, loại bỏ tin trùng và tạo bản tin tóm tắt hằng ngày hoặc hằng tuần kèm đường dẫn nguồn để kiểm chứng.
4. **Dịch tài liệu nhưng giữ nguyên cấu trúc file:** Kết hợp tool và AI để đọc từng thành phần, dịch nội dung rồi thay thế văn bản đúng vị trí, giữ nguyên bố cục, bảng biểu, hình ảnh và định dạng; người dùng kiểm tra lại thuật ngữ kỹ thuật trước khi xuất file.
5. **Kiểm tra và xử lý cảnh báo hệ thống:** Xây dựng AI Workflow tổng hợp cảnh báo, loại bỏ cảnh báo trùng, phân loại theo mức độ nghiêm trọng, đối chiếu lịch sử sự cố và gợi ý nguyên nhân hoặc hướng xử lý; kỹ sư kiểm tra và quyết định hành động cuối cùng.

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi:
- Ý dùng được:
- Ý bỏ vì không phải pain thật:

**Self-check Phase 1:**
- [*] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [*] Dùng ít nhất 3/4 lăng kính
- [*] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — [Tên problem]

```text
Problem 1 câu:

Actor:

Thời điểm / bối cảnh:

Current workflow 3-7 bước:
1.
2.
3.
4.
5.

Bottleneck:

Impact:

Success metric:

Non-AI alternative:

AI hypothesis:

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — ___ phút

[1 ...: __'] → [2 ...: __'] → [3 ...: __'] → [4 ...: __']  <-- bottleneck

FUTURE STATE — ___ phút

[1 ...: __'] → [2 ...: __'] → [3 ... review: __']  <-- human boundary

Fallback: nếu AI sai thì ...
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — [Tên problem]

```text
Problem 1 câu:

Actor:

Thời điểm / bối cảnh:

Current workflow 3-7 bước:
1.
2.
3.
4.
5.

Bottleneck:

Impact:

Success metric:

Non-AI alternative:

AI hypothesis:

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — ___ phút

[1 ...] → [2 ...] → [3 ...]  <-- bottleneck

FUTURE STATE — ___ phút

[1 ...] → [2 ...] → [3 ... review]  <-- human boundary

Fallback: ...
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — [Tên problem]

```text
Problem 1 câu:

Actor:

Thời điểm / bối cảnh:

Current workflow 3-7 bước:
1.
2.
3.
4.
5.

Bottleneck:

Impact:

Success metric:

Non-AI alternative:

AI hypothesis:

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — ___ phút

[1 ...] → [2 ...] → [3 ...]  <-- bottleneck

FUTURE STATE — ___ phút

[1 ...] → [2 ...] → [3 ... review]  <-- human boundary

Fallback: ...
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text

```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text

```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text

```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra:
- Tôi sửa gì:

### Self-check nộp phần 01
- [ ] Có 5+ problems + top 3 Cards đủ field
- [ ] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [ ] Đã chọn 1 card pitch + câu hỏi challenge
