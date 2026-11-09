# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: FreeFire
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Sinh viên CNTT năm cuối mất ~45 phút/CV để chỉnh mô tả đồ án và kỹ năng khớp từng JD khi ứng tuyển Fresher/Junior.
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nhân | Khi nhận tài liệu dài mà deadline gần, xác định phần kiến thức liên quan trực tiếp đến yêu cầu bài để đọc trước | Sinh viên đại học chuẩn bị bài tập/buổi học | Bước đối chiếu yêu cầu để chọn thứ tự đọc (chưa đo) | Chưa ghi nhận. *(Câu tác giả muốn nhóm hỏi: bước chọn phần đọc thật sự mất thời gian, hay do chưa hiểu rõ yêu cầu bài?)* |
| 2 | Nhân | Khi gặp lại nội dung chưa hiểu hoặc đã quên, tìm lại và nắm ý cần dùng mà không đọc lại cả phần dài | Sinh viên đang làm bài hoặc ôn tập | Đọc lại đoạn liên quan nhưng chưa nắm ý (chưa đo) | Chưa ghi nhận |
| 3 | Nhân | Khi học một khái niệm từ nhiều nguồn, xác định điểm thống nhất và khác biệt giữa các nguồn | Sinh viên làm bài cần đối chiếu nguồn | So sánh nội dung giữa các nguồn (chưa đo) | Chưa ghi nhận |
| 4 | Hải Anh | Khi các thành viên hiểu khác nhau về một tính năng, thống nhất hành vi mong đợi và điều kiện hoàn thành | Thành viên frontend, backend, kiểm thử | Đọc lại yêu cầu và trao đổi, ~40 phút/lần | Chưa ghi nhận. *(Câu tác giả muốn nhóm hỏi: nếu đã có tài liệu yêu cầu chung và điều kiện hoàn thành rõ, hiểu sai còn xảy ra không?)* |
| 5 | Hải Anh | Khi danh sách tính năng vượt thời gian và nhân lực, xác định phần tối thiểu để kiểm chứng giá trị chính | Nhóm trưởng và thành viên phát triển | Tranh luận ưu tiên và cắt giảm, ~60 phút/buổi | Chưa ghi nhận |
| 6 | Hải Anh | Khi tìm hiểu các sản phẩm tương tự, xác định họ làm tốt phần nào và người dùng còn vướng ở đâu | Thành viên nghiên cứu sản phẩm tương tự | Đối chiếu thông tin giữa các sản phẩm, ~60 phút | Chưa ghi nhận |
| 7 | Hiệu | Khi tìm thấy JD phù hợp, chỉnh mô tả đồ án và kỹ năng trong CV khớp JD mà không mất cả buổi tối | Sinh viên CNTT năm cuối ứng tuyển Fresher/Junior | Viết lại bullet mô tả đồ án, ~20 phút (tổng 45 phút/CV) | Chưa ghi nhận. *(Câu tác giả muốn nhóm hỏi: 2–3 bản CV cố định đã đủ qua vòng lọc chưa, hay cần viết lại theo từng JD?)* |
| 8 | Hiệu | Khi mở hàng chục tin tuyển dụng mỗi tối, xác định nhanh tin đúng tech stack và nhận dưới 1 năm kinh nghiệm | Sinh viên CNTT năm cuối tìm việc | Đọc chi tiết 25–30 JD, ~30 phút (tổng 50 phút/tối) | Chưa ghi nhận |
| 9 | Hiệu | Khi nhận lời mời phỏng vấn, nắm sản phẩm, tech stack và câu hỏi thường gặp để ôn trọng tâm | Sinh viên chuẩn bị phỏng vấn kỹ thuật | Tổng hợp câu hỏi ôn từ thông tin rời rạc, ~25 phút (tổng 60 phút) | Chưa ghi nhận |
| 10 | Dũng | Khi nhận 100–200 ca dự đoán sai từ production mỗi tuần, phân loại nhanh nguyên nhân để quyết định hướng retrain | AI Engineer duy trì chất lượng model (phối hợp QA, đội gán nhãn) | Xem mẫu và gom pattern viết nhận định, ~75/120 phút | Chưa ghi nhận. *(Câu tác giả muốn nhóm hỏi: thế nào là phân nhóm lỗi "đủ chính xác", và tránh "mù kép" khi dùng AI bắt lỗi AI ra sao?)* |
| 11 | Dũng | Khi Backend tích hợp hoặc cập nhật AI API, có tài liệu đặc tả luôn khớp code kèm ví dụ payload/mã lỗi | AI Engineer và Backend Dev | Viết mô tả tham số và giải thích lại trên Slack, ~45/60 phút | Chưa ghi nhận |
| 12 | Dũng | Khi kết thúc sprint, gom chi phí GPU/API và container lãng phí về một bảng cho Engineering Manager | AI Engineer và Engineering Manager | Đối chiếu container với chủ job, ~15/45 phút | Chưa ghi nhận |

*Cột phản biện: các câu in nghiêng là câu mỗi tác giả chuẩn bị cho card muốn pitch nhất, chưa phải câu đã được ai hỏi tại buổi pitch. Cần thay bằng câu hỏi thực tế (ghi rõ ai hỏi) sau buổi pitch.*

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Đọc, lọc, đối chiếu nhiều nguồn | #1, #3, #6, #8 | Tài liệu dài, không đồng nhất; phải đọc nhiều để tìm đúng phần cần dùng |
| B — Soạn lại nội dung cho người nhận cụ thể | #7, #9, #11, #12 | Đã có dữ liệu gốc (đồ án, JD, code, billing), phải viết lại theo yêu cầu của người đọc (HR, interviewer, Backend, EM) |
| C — Thống nhất yêu cầu và phạm vi trong nhóm | #4, #5 | Thành viên hiểu khác nhau hoặc tranh luận lâu mới chốt được |
| D — Chẩn đoán và tìm lại | #10, #2 | Phải quay lại từng mẫu hoặc từng đoạn cụ thể để tìm nguyên nhân hay ý cần dùng |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian sinh viên CNTT dành cho việc ứng tuyển mà hồ sơ vẫn đúng sự thật
├── Opportunity A: Mỗi JD đòi từ khóa khác nhau, phải viết lại mô tả đồ án cho từng CV (bước tốn nhất, ~20 phút/CV)
├── Opportunity B: Mỗi tối phải đọc 25–30 JD không cùng cấu trúc để tìm 2–3 JD nộp được
├── Opportunity C: Chuẩn bị phỏng vấn phải gom thông tin rời rạc (JD, website công ty, review)
└── Opportunity D: Chưa biết CV sau khi chỉnh có thật sự qua vòng lọc tốt hơn không
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- "Công cụ AI tự viết CV"
- "Agent tự quét JD và tự nộp đơn"

### 2.4. Chấm điểm shortlist (1–5)

Shortlist gồm 4 card mà mỗi thành viên chọn pitch (#7, #10, #4, #1). Tối đa 35 điểm.

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #7 Chỉnh CV theo JD (Hiệu) | 5 | 5 | 4 | 4 | 5 | 5 | 5 | **33** |
| #10 Phân loại ca lỗi production (Dũng) | 5 | 5 | 4 | 4 | 2 | 5 | 2 | 27 |
| #4 Hiểu khác nhau về yêu cầu tính năng (Hải Anh) | 4 | 4 | 2 | 3 | 4 | 3 | 5 | 25 |
| #1 Xác định phần kiến thức cần ưu tiên (Nhân) | 4 | 3 | 1 | 2 | 4 | 3 | 5 | 22 |

**Candidate được chọn:** #7 — Chỉnh CV khớp với từng JD (Problem Card #1 của Hiệu).

**Vì sao chọn:** Quy trình 6 bước có số phút, bottleneck rõ ở bước viết lại bullet đồ án (~20 phút). Baseline do Hiệu tự bấm giờ 5 lần gần nhất: trung bình 45 phút/CV, tuần qua 6 CV = 270 phút. Cả 4 thành viên là sinh viên, hiểu quy trình ứng tuyển và có thể phỏng vấn, poll bạn cùng lớp ở CP4. So sánh được đủ 4 mức: No AI (3 bản CV cố định + ngân hàng câu mô tả đồ án), Rule, Workflow (AI nháp bullet, sinh viên duyệt), Agent (loại vì rủi ro tự nộp đơn). Điểm trừ: số liệu mới của 1 người, cần kiểm chứng thêm.

**Vì sao loại các candidate còn lại:**

- **#10 (Dũng):** chi tiết nhất nhóm, baseline 115 và 130 phút trên 2 batch, nhưng cần log production, ảnh/text gốc và đội QA thật; nhóm chưa vận hành hệ thống production nên khó kiểm chứng và khó pilot. Rủi ro "AI bắt lỗi của AI" khó kiểm chứng trong thời gian lab.
- **#4 (Hải Anh):** gần trải nghiệm đồ án của nhóm, nhưng số liệu trong bài ghi là "minh họa, chưa xác nhận", và bản AI phản biện cho thấy có thể giải bằng tài liệu yêu cầu chung + checklist nên khó chứng minh cần AI.
- **#1 (Nhân):** chưa có số đo nào (mọi số phút còn là "..."), quy trình mới là bản suy ra, chưa đủ cơ sở xác định bottleneck thực.

**Xử lý bất đồng (nếu có):** *(Bản nháp dựa trên khác biệt có thật giữa các bài cá nhân, chưa phải cuộc tranh luận đã xảy ra. Cần thay bằng bất đồng thật của nhóm.)* Bài #10 của Dũng có chi tiết kỹ thuật và baseline đầy đủ nhất nên có thể được đề xuất chọn. Nhóm nhận thấy dữ liệu production không kiểm chứng được trong lab nên ghi #10 vào hướng tiếp theo, và chọn #7 vì có baseline đo được ngay và có thể phỏng vấn người thật. Các candidate #8 và #9 (cùng chuỗi ứng tuyển) cũng giữ cho vòng sau.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Sinh viên CNTT khác cũng mất trên 30 phút/CV khi chỉnh CV theo từng JD | Value | 5 | 2 | ✅ |
| 2 | Bước tốn nhất là viết lại bullet mô tả đồ án, không phải đọc JD hay căn chỉnh layout | Value | 5 | 2 | ✅ |
| 3 | Chỉnh CV riêng cho từng JD thật sự cần thiết; 3 bản CV cố định + ngân hàng câu mô tả chưa đủ | Value | 5 | 1 | ✅ |
| 4 | Sinh viên sẵn sàng dùng bản nháp AI và tự kiểm từng dòng trước khi nộp | Usability | 4 | 1 | ✅ |
| 5 | Có thể giữ bản nháp chỉ dựa trên đồ án có thật, không bịa kỹ năng hay số liệu | Feasibility | 4 | 3 | Kiểm trong pilot |
| 6 | Đưa dữ liệu đồ án và CV vào công cụ AI chấp nhận được về riêng tư và chi phí (gói free có giới hạn) | Viability | 3 | 3 | Kiểm sau |

### 3.2. Kiểm chứng

Cách đã dùng: **Log (tự bấm giờ, dữ liệu thật)** và **Phỏng vấn nội bộ nhóm** theo The Mom Test.

**Bằng chứng thật (từ bài cá nhân của Hiệu, CP1–CP2):** tự bấm giờ 5 lần sửa CV gần nhất, trung bình 45 phút/CV; tuần trước nộp 6 công ty, tổng 270 phút. Quy trình 6 bước: đọc JD 5' → mở CV gốc và GitHub 3' → chọn đồ án 5' → viết lại bullet 20' → căn layout và xuất PDF 7' → nộp và ghi Sheets 5'.

**Interview snapshot — buổi 1 : Hải Anh**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên làm đồ án nhóm, đang xin thực tập |
| Câu nói đáng nhớ nhất (nguyên văn) | "Phần lâu nhất là viết lại câu chữ, vì mình sợ viết quá lên so với những gì mình làm thật." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tuần trước nộp CV cho một công ty sản phẩm; đọc JD rồi viết lại phần mô tả đồ án cho khớp từ khóa |
| Hiện đang xử lý bằng cách nào (workaround)? | Sửa tay; thỉnh thoảng nhờ ChatGPT rồi đọc lại từng dòng (một lần AI tự thêm công nghệ chưa từng dùng) |
| Mất bao lâu, bao lần? | ~35–40 phút/CV (ước lượng theo trí nhớ); không nhớ rõ tần suất |
| Insight / opportunity rút ra | Pain nằm ở bước viết lại bullet và nỗi lo viết sai sự thật; cần bước duyệt từng dòng |

**Interview snapshot — buổi 2 : Nhân**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên, mới bắt đầu nộp CV, ít đơn |
| Câu nói đáng nhớ nhất (nguyên văn) | "Cái mình mất thời gian hơn là đọc JD để quyết định có nộp không." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Đầu học kỳ nộp thử 2 công ty, dùng một CV chung, chỉ sửa phần giới thiệu |
| Hiện đang xử lý bằng cách nào (workaround)? | Một CV chung; từng nhờ AI nhận xét CV chung, không dùng để viết lại theo JD |
| Mất bao lâu, bao lần? | ~10–15 phút/lần sửa phần giới thiệu (ước lượng); 2 đơn |
| Insight / opportunity rút ra | Người nộp ít đơn không coi viết lại bullet là bottleneck; pain nghiêng về đọc và lọc JD (Opportunity B) |

**Interview snapshot — buổi 3 : Dũng**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Kỹ sư AI đã đi làm, từng đổi việc |
| Câu nói đáng nhớ nhất (nguyên văn) | "Mình xóa các số liệu mà mình không nhớ đã làm. Mình không muốn bị hỏi ngược lại trong phỏng vấn." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Một lần JD yêu cầu sâu về RAG, bản CV cố định chưa nhấn phần đó, phải viết lại |
| Hiện đang xử lý bằng cách nào (workaround)? | 2 bản CV cố định + file câu mô tả dự án (tương đương "bullet bank") |
| Mất bao lâu, bao lần? | ~10–15 phút với bản cố định; ~30 phút khi JD lệch bản cố định (ước lượng) |
| Insight / opportunity rút ra | No AI (bản cố định + bullet bank) đủ cho phần lớn trường hợp; chỉ JD lệch mới tốn thời gian. Người dùng tự nhận ra rủi ro AI bịa số liệu |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Tự bấm giờ (Hiệu) | 5 lần, 1 người | Trung bình 45 phút/CV; bước viết lại bullet ~20 phút | Chưa có; dữ liệu của một người |
| Phỏng vấn nội bộ | 3 | 1/3 (Hải Anh) sửa từng JD, ~35–40 phút, nghẽn ở viết lại bullet; 2/3 nêu nỗi lo AI thêm nội dung không đúng sự thật | 2/3 không sửa bullet theo từng JD: Nhân dùng CV chung (pain ở đọc JD); Dũng dùng bản cố định + bullet bank, chỉ 10–15 phút |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** thu hẹp actor thành "sinh viên nộp nhiều đơn và sửa CV riêng cho từng JD"; giữ phương án No AI (bản cố định + bullet bank) cho người nộp ít đơn; đặt "AI không tự thêm công nghệ hay số liệu không có trong dữ liệu đồ án" làm boundary bắt buộc; thu hẹp hướng giải từ "xây công cụ AI viết CV" thành "soạn nháp bullet từ dữ liệu đồ án thật, sinh viên duyệt từng dòng". Giả định #3 (bản cố định chưa đủ) vẫn chưa đủ bằng chứng.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Teal (AI Resume Builder + Job Matcher) | https://www.tealhq.com/free | Bước 1, 3, 4: dán JD, tìm kỹ năng/từ khóa nhà tuyển dụng cần, gợi ý chỉnh nội dung CV; có job tracker (liên quan bước 6) | Trang chính thức nêu: phân tích CV theo JD, chấm điểm match, gợi ý từ khóa; có gói miễn phí | Trang giá (https://tealhq.com/resume-builder) ghi gói free chỉ có AI credits giới hạn, phân tích và so khớp từ khóa nâng cao ở gói trả phí. Match Score dựa trên từ khóa, không kiểm tra nội dung có đúng sự thật không | Thị trường đã có sản phẩm làm đúng bước 4, không nên tự xây từ đầu. Có thể thử gói free để đo thời gian thật cho phương án Workflow |
| Jobscan (Match Report) | https://jobscan.co/resume-matcher | Bước 1, 3: so CV với JD, liệt kê kỹ năng cứng/mềm còn thiếu | Trang chính thức: Match Report miễn phí 5 lần quét, chỉ ra kỹ năng thiếu và số lần xuất hiện | Chính trang https://www.jobscan.co/resume-checker nói ATS thật không chấm điểm CV, Match Rate chỉ để hình dung. Chấm theo từ khóa nên dễ dẫn đến nhồi từ khóa | Dùng như bước **Rule** (kiểm từ khóa thiếu), không dùng điểm này làm metric chất lượng. Metric chất lượng của nhóm cần cách đo khác (đúng sự thật, mentor/bạn đọc) |
| Kickresume (AI Writer) | https://www.kickresume.com/pricing | Bước 4: tạo hoặc viết lại nội dung CV từ job title và tin tuyển dụng | Trang giá mô tả: nhập job title và job ad, AI tạo CV; có ATS Resume Checker trong gói trả phí | AI Writer thuộc gói trả phí. Rủi ro (suy ra từ cách hoạt động, chưa thử): khi AI tạo nội dung từ job title có thể sinh nội dung không đến từ đồ án thật | Nếu dùng công cụ kiểu "AI tạo CV", phải ép đầu vào là dữ liệu đồ án thật của sinh viên và duyệt từng dòng (boundary) |
| TopCV — tạo CV online theo mẫu | https://www.topcv.vn/cach-tao-cv-online-tren-topcv | Bước 5: căn layout, xuất PDF | Trang hướng dẫn nêu có gần 70 mẫu theo style và mẫu theo vị trí ứng tuyển; đây là phương án No AI cho phần trình bày | Mẫu giải quyết layout, không viết lại mô tả đồ án theo JD. Nhóm chưa tìm thấy trang chính thức xác nhận TopCV có tính năng AI chỉnh CV theo JD | Bước 5 (7 phút) giải bằng mẫu cố định; AI nên nhắm vào bước 4 |
| Cách dùng ChatGPT viết CV theo JD (pattern thủ công, bài hướng dẫn tiếng Việt) | https://findskill.ai/vi/blog/ai-viet-cv-xin-viec-2026-huong-dan-tieng-viet/ ; thêm: https://www.rezi.ai/posts/rezi-alternatives | Bước 4: dán JD và dữ liệu thật, nhờ AI viết lại bullet | Không cần công cụ mới; bài hướng dẫn nêu cách làm: dán nguyên JD, cung cấp dữ liệu thật, đọc lại từng dòng và xóa số liệu không nhớ. Blog của Rezi cũng nhắc nội dung chỉnh phải đúng kinh nghiệm thật | Cả hai là blog, không phải nghiên cứu; chưa có số liệu hiệu quả. Rezi là bên bán công cụ nên có thể thiên lệch | Mức **Workflow** có thể bắt đầu bằng prompt chuẩn, chưa cần xây gì. Cách làm này trùng với boundary mà nhóm đã đề xuất (AI không bịa, sinh viên duyệt trước khi nộp) |

**Kết luận research:**

```text
Bước viết lại bullet theo JD (bottleneck) đã có công cụ hỗ trợ (Teal, Kickresume) hoặc làm được bằng prompt chuẩn.
Không có lý do tự xây một công cụ mới.
Hướng hợp lý: Rule kiểm từ khóa thiếu (Jobscan/Teal free) -> AI nháp bullet từ dữ liệu đồ án thật -> sinh viên duyệt từng dòng -> sinh viên nộp.
Chưa kiểm chứng: nháp AI có thật sự giảm từ 45 xuống dưới 15 phút/CV hay không (cần pilot, CP6).
```

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
