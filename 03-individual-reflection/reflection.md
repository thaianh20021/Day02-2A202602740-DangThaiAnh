# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Đặng Thái Anh
- Mã học viên: 2A202602740
- Nhóm: Chưa bổ sung số/tên nhóm
- Candidate problem nhóm chọn: Chuẩn hóa Git workflow, commit và merge code giữa các developer trước khi release production

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Tôi liệt kê 5 vấn đề từ công việc kỹ thuật và viết chi tiết 3 Problem Cards về dữ liệu Power BI, tổng hợp thông tin đa kênh và dịch file giữ nguyên cấu trúc. | Nhóm có thêm các candidate gắn với workflow thật, có actor, bottleneck, metric và fallback để so sánh. |
| Pitch Problem Card | Tôi chuẩn bị nội dung pitch cho bài SmartPV/Power BI, tập trung vào bước làm sạch dữ liệu thủ công và phần người thật phải review. | Candidate được trình bày theo problem trước, solution sau và tránh gọi toàn bộ quy trình là Agent. |
| Challenge bài của bạn khác | Tôi dùng các câu hỏi về actor, tần suất, baseline, dữ liệu sẵn có, hậu quả khi AI sai và phương án non-AI. | Các candidate quá rộng hoặc chỉ cần rule/template được nhận diện sớm hơn. |
| Gom trùng / cluster | Tôi điều phối việc gom 17 candidate thành 4 cụm: phát triển phần mềm, fanpage/CS, tài liệu/thông tin và dữ liệu vận hành/quản lý thời gian. | Nhóm nhìn rõ các ý trùng nhau và rút xuống shortlist 3 bài thay vì tranh luận trên toàn bộ danh sách. |
| Chọn candidate problem | Tôi dẫn việc chấm actor, workflow, evidence, impact, khả năng làm trong lab, Rule/Workflow/Agent và hiểu biết domain. | Nhóm chốt bài chuẩn hóa Git workflow vì có thể pilot trực tiếp và phù hợp năng lực kỹ thuật chung. |
| Validation / research | Tôi tổng hợp kết quả nhóm phỏng vấn developer/Tech Lead, survey sinh viên CNTT và phân tích 30 pull request; đồng thời đối chiếu các giải pháp Commitlint, branch protection và Conventional Commits. | Nhóm xác định pain nằm ở commit thiếu ý nghĩa, PR chưa đủ thông tin và thời gian Tech Lead phải rà soát, thay vì chỉ nói chung rằng Git khó dùng. |
| Workflow nhóm | Tôi cùng nhóm mô tả luồng hiện tại từ feature branch đến production và luồng tương lai có rule, CI, review cùng production approval. | Bottleneck leader kiểm tra thủ công và human boundary trước merge/production được thể hiện rõ. |
| Problem Statement | Tôi ghép actor, workflow, bottleneck, impact, metric và boundary thành Problem Statement v0/v1. | Problem được thu hẹp từ “quản lý Git” thành kiểm soát branch, commit, PR, merge và release. |
| Rule / Workflow / Agent | Tôi phản biện việc dùng Agent và đề xuất Workflow + Rule; AI chỉ tóm tắt diff, đề xuất commit hoặc giải thích conflict. | Giải pháp dùng tính năng native trước, không cấp cho AI quyền sửa, approve, merge hoặc push production. |
| Decision | Tôi đề xuất Go cho pilot nhỏ nhưng chưa Go cho tự động merge hoặc production deployment. | Nhóm có pilot, metric, owner, fallback và điều kiện rollback rõ ràng. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Tôi là người điều phối quá trình từ danh sách candidate đến quyết định cuối, đồng thời trực tiếp siết lại boundary để AI không có quyền merge hoặc push production. Dấu tay rõ nhất của tôi là bảng hội tụ, workflow trước/sau và lập luận chọn Workflow + Rule thay vì Agent.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Gợi ý các pain lặp lại từ công việc kỹ thuật và phản biện độ phù hợp AI. | AI giúp mở rộng góc nhìn và chuyển mô tả công việc thành actor, workflow, bottleneck. | Một số ý quá rộng hoặc gọi mọi tự động hóa là Agent dù chưa có evidence. | Tôi chỉ giữ 5 pain gắn với công việc thật và tách rule/workflow khỏi AI. |
| Problem Card | Gợi ý cấu trúc current/future workflow, metric và fallback cho 3 card. | AI giúp tôi không bỏ sót success metric, non-AI alternative và human boundary. | AI có xu hướng tự đặt thời gian hoặc tỷ lệ hiện tại khi tôi chưa đo. | Tôi thay số chưa có bằng T1/T2/T3 và ghi cách thu thập baseline. |
| Workflow | Hỗ trợ mô tả các bước Git từ feature branch đến production. | AI giúp tách actor, input, output, handoff và bottleneck theo từng bước. | Workflow ban đầu có quá nhiều tính năng AI và chưa ưu tiên khả năng native của Git platform. | Tôi rút về branch rule, PR, CI, review, merge và production approval. |
| Research | Gợi ý các pattern như protected branch, required checks, PR template và Conventional Commits. | AI giúp xác định đúng nhóm tài liệu chính thức cần kiểm tra. | AI không thay thế được việc xác nhận tính năng, quyền truy cập hoặc giới hạn theo gói dịch vụ. | Tôi chỉ đưa tài liệu chính thức vào report và ghi rõ những giả định chưa kiểm chứng. |
| Problem Statement | Tạo bản nháp từ mô tả “push và merge code”. | AI giúp viết actor, bottleneck, impact và boundary thành câu đầy đủ. | Bản đầu thiên về solution và chưa phân biệt lỗi quy trình với lỗi chất lượng code. | Tôi thu hẹp pain vào quy tắc branch/commit/PR và bước kiểm tra thủ công của leader. |
| Rule / Workflow / Agent | So sánh ba mức giải pháp trên cùng một bài toán. | AI giúp chỉ ra phần đúng/sai rõ nên dùng rule và phần nhiều bước nên dùng workflow. | AI ban đầu gợi ý bot/Agent có quyền thao tác repository quá sớm. | Tôi bỏ quyền tự hành động, chỉ giữ AI assistant không có quyền merge hoặc production. |
| Decision | Gợi ý pilot, metric và điều kiện rollback. | AI giúp tạo checklist đo thời gian, số lần sửa và tỷ lệ PR qua checks. | AI dễ trộn baseline từ validation với mục tiêu pilot hoặc diễn đạt kết quả quá chắc chắn. | Tôi phân biệt số liệu nhóm đã ghi nhận với mục tiêu sau hai tuần và giữ quyền quyết định merge/rollback cho Tech Lead. |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Khi nghe các candidate của mọi người, tôi nhận ra một bài nghe “AI” hơn chưa chắc đã là bài phù hợp nhất để làm. Với vai trò leader, phần khó nhất của tôi là giữ cuộc thảo luận đi từ problem, workflow và evidence thay vì nhảy thẳng sang Agent. Ban đầu nhóm cân nhắc FAQ fanpage vì có số liệu rõ, nhưng sau đó chọn Git workflow do nhiều thành viên hiểu domain và có thể pilot trực tiếp trên repository. Kết quả interview, survey và phân tích pull request giúp nhóm thu hẹp pain vào commit thiếu ý nghĩa, PR chưa đủ thông tin và thời gian Tech Lead phải rà soát. Khi viết Problem Statement, boundary khó hơn metric vì AI có thể hỗ trợ tóm tắt nhưng không nên có quyền quyết định merge hoặc production release. Tôi đóng góp rõ nhất ở phần gom candidate, tổ chức bảng score và tách giải pháp thành Rule, Workflow và AI assistant. AI giúp tôi viết cấu trúc nhanh hơn nhưng đôi khi mở rộng phạm vi hoặc diễn đạt kết quả quá chắc chắn. Tôi đã sửa bằng cách phân biệt baseline với mục tiêu pilot và giữ người thật ở các bước review, merge và release. Nếu làm lại, tôi sẽ yêu cầu mỗi thành viên mang theo log, pull request hoặc quote thật ngay từ lúc pitch để rút ngắn thời gian validation. Tôi cũng sẽ chốt tiêu chí chọn bài trước khi nghe solution để nhóm ít bị ảnh hưởng bởi độ “ngầu” của công nghệ.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [ ] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (chỉ check sau khi thực hiện thật)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI

