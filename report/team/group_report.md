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

![Cây OST CP3: giảm thời gian ứng tuyển mà hồ sơ vẫn đúng sự thật, với bốn nhánh opportunity; nhánh A chỉnh CV theo JD được chọn](../assets/cp3-ost.png)

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

**Nhóm đã sửa problem thế nào sau kiểm chứng:** thu hẹp actor thành "sinh viên nộp nhiều đơn và sửa CV riêng cho từng JD"; giữ phương án No AI (bản cố định + bullet bank) cho người nộp ít đơn; bổ sung vào quy trình bước **lọc các JD phù hợp với thông tin (kỹ năng, dự án) hiện có của người dùng** trước khi chỉnh CV và đặt "AI không tự thêm công nghệ hay số liệu không có trong dữ liệu đồ án" làm boundary bắt buộc nhằm tránh việc bịa CV để khớp với JD; thu hẹp hướng giải từ "xây công cụ AI viết CV" thành "soạn nháp bullet từ dữ liệu đồ án thật cho các JD đã lọc phù hợp, sinh viên duyệt từng dòng". Giả định #3 (bản cố định chưa đủ) vẫn chưa đủ bằng chứng.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Teal (AI Resume Builder + Job Matcher) | https://www.tealhq.com/free | Bước lọc JD, so khớp từ khóa và nháp bullet: dán JD, tìm kỹ năng/từ khóa nhà tuyển dụng cần, gợi ý chỉnh nội dung CV; có job tracker | Trang chính thức nêu: phân tích CV theo JD, chấm điểm match, gợi ý từ khóa; có gói miễn phí | Trang giá (https://tealhq.com/resume-builder) ghi gói free chỉ có AI credits giới hạn, phân tích và so khớp từ khóa nâng cao ở gói trả phí. Match Score dựa trên từ khóa, không kiểm tra nội dung có đúng sự thật không | Thị trường đã có sản phẩm hỗ trợ so khớp và viết bullet, không nên tự xây từ đầu. Có thể thử gói free để hỗ trợ lọc JD và đo thời gian thật cho phương án Workflow |
| Jobscan (Match Report) | https://jobscan.co/resume-matcher | Bước lọc JD và so khớp từ khóa: đối chiếu CV/hồ sơ kỹ năng với JD, liệt kê kỹ năng cứng/mềm hiện có và còn thiếu | Trang chính thức: Match Report miễn phí 5 lần quét, chỉ ra kỹ năng thiếu và số lần xuất hiện | Chính trang https://www.jobscan.co/resume-checker nói ATS thật không chấm điểm CV, Match Rate chỉ để hình dung. Chấm theo từ khóa nên nếu JD lệch mà cố chạy theo điểm dễ dẫn đến nhồi từ khóa hoặc bịa kỹ năng | Dùng như bước **Rule** để lọc xem JD có khớp với kỹ năng/dự án hiện có không và xác định từ khóa cần nhấn mạnh; không dùng điểm này làm metric chất lượng để tránh bịa CV |
| Kickresume (AI Writer) | https://www.kickresume.com/pricing | Bước viết bullet: tạo hoặc viết lại nội dung CV từ job title và tin tuyển dụng | Trang giá mô tả: nhập job title và job ad, AI tạo CV; có ATS Resume Checker trong gói trả phí | AI Writer thuộc gói trả phí. Rủi ro (suy ra từ cách hoạt động, chưa thử): khi AI tạo nội dung từ job title có thể sinh nội dung không đến từ đồ án thật | Nếu dùng công cụ kiểu "AI tạo CV", phải lọc JD phù hợp trước, ép đầu vào là dữ liệu đồ án thật của sinh viên và duyệt từng dòng (boundary) |
| TopCV — tạo CV online theo mẫu | https://www.topcv.vn/cach-tao-cv-online-tren-topcv | Bước căn layout, xuất PDF | Trang hướng dẫn nêu có gần 70 mẫu theo style và mẫu theo vị trí ứng tuyển; đây là phương án No AI cho phần trình bày | Mẫu giải quyết layout, không viết lại mô tả đồ án theo JD. Nhóm chưa tìm thấy trang chính thức xác nhận TopCV có tính năng AI chỉnh CV theo JD | Bước căn layout (7 phút) giải bằng mẫu cố định; AI nên nhắm vào bước viết lại bullet |
| Cách dùng ChatGPT viết CV theo JD (pattern thủ công, bài hướng dẫn tiếng Việt) | https://findskill.ai/vi/blog/ai-viet-cv-xin-viec-2026-huong-dan-tieng-viet/ ; thêm: https://www.rezi.ai/posts/rezi-alternatives | Bước viết lại bullet: dán JD và dữ liệu thật, nhờ AI viết lại bullet | Không cần công cụ mới; bài hướng dẫn nêu cách làm: dán nguyên JD, cung cấp dữ liệu thật, đọc lại từng dòng và xóa số liệu không nhớ. Blog của Rezi cũng nhắc nội dung chỉnh phải đúng kinh nghiệm thật | Cả hai là blog, không phải nghiên cứu; chưa có số liệu hiệu quả. Rezi là bên bán công cụ nên có thể thiên lệch | Mức **Workflow** có thể bắt đầu bằng prompt chuẩn, chưa cần xây gì. Cách làm này trùng với boundary mà nhóm đã đề xuất (AI không bịa, sinh viên duyệt trước khi nộp) |

**Kết luận research:**

```text
Bước viết lại bullet theo JD (bottleneck) đã có công cụ hỗ trợ (Teal, Kickresume) hoặc làm được bằng prompt chuẩn.
Không có lý do tự xây một công cụ mới.
Hướng hợp lý: AI lọc JD phù hợp với thông tin (kỹ năng, dự án) hiện có -> Rule kiểm từ khóa thiếu (Jobscan/Teal free) -> AI nháp bullet từ dữ liệu đồ án thật -> sinh viên duyệt từng dòng -> sinh viên nộp.
Chưa kiểm chứng: quy trình có AI hỗ trợ có thật sự giảm từ 45 xuống dưới 15 phút/CV hay không (cần pilot, CP6).
```

---


## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Thời gian lấy từ số tự bấm giờ của Hiệu (5 lần sửa CV gần nhất, trung bình 45 phút/CV; tuần trước nộp 6 CV).

```text
HIỆN TẠI — 6 bước, 45 phút/CV, 6/6 bước thủ công (chưa có bước lọc JD theo hồ sơ năng lực chuẩn hóa)

[1 Đọc JD, gạch từ khóa: 5'] → [2 Mở CV gốc và GitHub: 3'] → [3 Chọn đồ án khớp JD: 5']
→ [4 Viết lại bullet mô tả đồ án theo JD: 20'] ← BOTTLENECK
→ [5 Căn layout 1 trang, xuất PDF: 7'] → [6 Nộp đơn, ghi vào Google Sheets: 5']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Sinh viên | JD đã chọn (từ ITviec, LinkedIn, TopCV...) | Danh sách yêu cầu và từ khóa (tech stack, kỹ năng, domain) | 5 phút/CV; ~6 CV/tuần | Gạch chân tay; chưa có bước lọc JD tự động theo hồ sơ kỹ năng/dự án hiện có nên dễ giữ lại cả JD lệch năng lực |
| 2 | Sinh viên | CV gốc (Overleaf/Word/Canva), danh sách đồ án trên GitHub | CV gốc và danh sách đồ án đã mở | 3 phút/CV | |
| 3 | Sinh viên | Từ khóa JD, danh sách đồ án | Đồ án khớp nhất với JD | 5 phút/CV | Dựa vào trí nhớ và README; nếu JD đòi kỹ năng chưa có trong đồ án, dễ phát sinh tâm lý cố viết ép cho khớp JD |
| 4 | Sinh viên | Từ khóa JD, mô tả đồ án đã chọn | Các bullet mới khớp từ khóa JD mà vẫn đúng sự thật | **20 phút/CV** | **Bottleneck**: phải cân nhắc câu chữ nổi bật kỹ năng JD cần; nếu nhờ AI viết trực tiếp từ JD chưa lọc thì rất dễ bịa CV |
| 5 | Sinh viên | Bullet mới, CV gốc | CV 1 trang A4 dạng PDF | 7 phút/CV | Kiểm lỗi chính tả, căn layout |
| 6 | Sinh viên | PDF CV, thông tin công ty, link JD | Hồ sơ đã nộp; dòng mới trong Google Sheets | 5 phút/CV | Ghi bản CV đã gửi |

**Bottleneck chính:** Bước 4, viết lại bullet mô tả đồ án, 20 phút trên tổng 45 phút (khoảng 44% thời gian mỗi CV). Ngoài ra, việc thiếu bước lọc JD dựa trên thông tin (kỹ năng, dự án) hiện có ngay từ đầu khiến người dùng hoặc AI dễ cố bịa thêm kỹ năng vào CV để khớp với những JD không phù hợp.

### 4.2. Quy trình tương lai

Các số phút dưới đây là **kỳ vọng chưa đo**, cần kiểm bằng pilot. Nhóm bổ sung thêm **1 bước do AI thực hiện: lọc các JD phù hợp với thông tin (kỹ năng, dự án) hiện có của người dùng** ngay đầu quy trình (nâng tổng số bước lên **7 bước**), nhằm loại bỏ sớm các JD lệch năng lực và tránh việc bịa CV để khớp với JD.

```text
TƯƠNG LAI — 7 bước, khoảng 14 phút/CV (kỳ vọng), 3/7 bước thủ công (2 bước AI, 2 bước Rule)

[1 Lọc các JD phù hợp với thông tin (kỹ năng, dự án) hiện có của người dùng: 1'] ← AI (lọc JD chống bịa CV)
→ [2 Dán JD đã lọc vào công cụ so khớp từ khóa, đọc từ khóa còn thiếu: 1']       ← RULE
→ [3 Chọn đồ án khớp JD từ danh sách đồ án đã chuẩn bị sẵn: 2']                 ← CON NGƯỜI
→ [4 Nháp 3–5 bullet từ đồ án đã chọn và JD, ghi đồ án nguồn: 1']               ← AI
→ [5 Duyệt từng dòng, sửa, xóa mọi nội dung không đúng: 5']                     ← CON NGƯỜI (điểm kiểm soát)
→ [6 Đưa bullet vào mẫu CV cố định, xuất PDF: 2']                               ← RULE (mẫu cố định)
→ [7 Sinh viên nộp, ghi vào Google Sheets: 2']                                  ← CON NGƯỜI

Chuẩn bị một lần (ngoài vòng lặp): tổng hợp hồ sơ thông tin hiện có của người dùng (danh sách kỹ năng thật, danh sách đồ án thật gồm vai trò, công nghệ, kết quả) và mẫu CV cố định.

BOUNDARY: Chỉ chỉnh CV cho các JD đã qua bước 1 (được AI đối chiếu là phù hợp với kỹ năng và dự án hiện có của người dùng);
          nếu JD yêu cầu kỹ năng/công nghệ cốt lõi mà người dùng không có thì loại bỏ JD ngay từ bước 1, tránh việc bịa CV để khớp với JD.
          AI không tự thêm kỹ năng, công nghệ hay số liệu không có trong danh sách đồ án;
          AI không tự nộp hồ sơ; chỉ dùng dữ liệu sinh viên cung cấp.
          Mỗi bullet phải ghi đồ án nguồn và được sinh viên duyệt trước khi xuất PDF.
PHƯƠNG ÁN QUAY VỀ: nếu nháp sai sự thật hoặc phải viết lại trên 50% ở 2 CV liên tiếp
          → bỏ nháp AI, dùng bản CV cố định + ngân hàng câu mô tả đồ án (No AI).
```

| Bước | Phân loại | Actor / Công cụ | Input | Output | Thời gian kỳ vọng | Mục đích & kiểm soát |
|---:|---|---|---|---|---:|---|
| 1 | **AI** | AI (Prompt đối chiếu JD với hồ sơ hiện có) | Danh sách JD + Thông tin hiện có của người dùng (kỹ năng, dự án thật) | Các **JD phù hợp** với năng lực hiện có (kèm lý do khớp / loại bỏ các JD đòi hỏi kỹ năng người dùng không có) | 1 phút/CV | **Cổng lọc chống bịa CV**: loại ngay các JD lệch hẳn với kỹ năng và dự án hiện có, tránh việc cố ép hoặc bịa CV để khớp với JD |
| 2 | **Rule** | Công cụ so khớp từ khóa (Jobscan/Teal free) | JD đã lọc ở bước 1 + CV gốc | Danh sách từ khóa trong JD còn thiếu trên CV gốc | 1 phút/CV | Xác định nhanh các từ khóa mà người dùng thực sự có trong dự án nhưng chưa đưa vào CV |
| 3 | **Con người** | Sinh viên | Từ khóa JD, danh sách đồ án đã chuẩn bị sẵn | Đồ án thật khớp nhất với JD | 2 phút/CV | Sinh viên chủ động chọn đúng dự án mình đã làm |
| 4 | **AI** | Prompt chuẩn / Công cụ AI | Đồ án đã chọn (dữ liệu thật) + Từ khóa JD | Bản nháp 3–5 bullet mô tả đồ án khớp JD, kèm trích dẫn đồ án nguồn | 1 phút/CV | Giải quyết bottleneck viết câu chữ mà chỉ đóng khung trong dữ liệu dự án hiện có |
| 5 | **Con người (HITL)** | Sinh viên | Bản nháp bullet của AI + Danh sách đồ án thật | Các bullet đã duyệt, sửa câu chữ và xóa mọi chi tiết phóng đại/sai lệch | 5 phút/CV | **Điểm kiểm soát chất lượng**: đảm bảo 100% thông tin đúng với kỹ năng và dự án thật |
| 6 | **Rule** | Mẫu CV cố định | Bullet đã duyệt + Mẫu CV cố định | File CV 1 trang A4 dạng PDF | 2 phút/CV | Tránh mất thời gian căn chỉnh lại bố cục |
| 7 | **Con người** | Sinh viên | File PDF CV, link JD | Hồ sơ đã nộp + Dòng theo dõi trên Google Sheets | 2 phút/CV | Sinh viên kiểm tra lần cuối và tự nộp |

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 6 | 7 | Bổ sung thêm **bước 1 (AI): Lọc các JD phù hợp với thông tin (kỹ năng, dự án) hiện có của người dùng** để tránh bịa CV khớp JD; đổi cách làm ở bước kiểm từ khóa, nháp bullet và xuất PDF |
| Tổng thời gian | 45' | khoảng 14' | Target chính: dưới 15'. Kỳ vọng chưa đo; baseline 45' chỉ từ 1 người |
| Số bước thủ công | 6/6 | 3/7 | 3 bước con người (chọn đồ án, duyệt nháp, nộp), 2 bước AI (lọc JD phù hợp, nháp bullet), 2 bước Rule (kiểm từ khóa, xuất PDF mẫu cố định) |
| Bottleneck chính | Viết lại bullet (20') | Sinh viên duyệt và sửa nháp (5') | Chấp nhận được vì là điểm kiểm soát chất lượng; nếu duyệt kỹ hơn dự kiến thì khó đạt target |
| Rủi ro mới phát sinh | Cố chỉnh CV cho cả JD lệch năng lực | AI lọc sót/nhầm JD; AI bịa kỹ năng hoặc số liệu; nhồi từ khóa; sinh viên duyệt qua loa | Xử lý bằng **bước 1 AI lọc JD dựa trên kỹ năng/dự án hiện có** (tránh bịa CV để khớp JD), kết hợp boundary, ghi đồ án nguồn cho từng bullet và tiêu chí đánh giá ở v1 |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên CNTT năm cuối ứng tuyển vị trí Fresher/Junior Backend/Fullstack, phải chỉnh CV theo từng JD |
| **Quy trình** | Lọc các JD phù hợp với thông tin (kỹ năng, dự án) hiện có → đọc JD và xác định từ khóa thiếu → mở CV gốc và danh sách đồ án → chọn đồ án khớp JD → viết lại bullet mô tả đồ án và kỹ năng theo từ khóa JD → căn layout 1 trang, xuất PDF → nộp và ghi vào Google Sheets |
| **Bottleneck** | Bước viết lại bullet mô tả đồ án mất khoảng 20 phút/CV (trên tổng 45 phút), vì phải chọn câu chữ nổi bật kỹ năng JD cần mà vẫn đúng sự thật |
| **Impact** | 45 phút/CV × 6 CV/tuần = 270 phút (4,5 giờ)/tuần/sinh viên; nhóm 4 người khoảng 18 giờ/tuần (ước tính của Hiệu); có lúc quá mệt nên nộp CV chung chung hoặc cố ép CV theo JD không thực sự phù hợp |
| **Success Metric** (baseline → target, cách đo) | Thời gian chỉnh một CV (với các JD đã lọc phù hợp): 45 phút (Hiệu tự bấm giờ 5 lần) → dưới 15 phút. Đo bằng sinh viên tự ghi giờ trên ít nhất 5 CV trong 2 tuần pilot. Đồng thời 100% bullet trong CV khớp với kỹ năng và đồ án có thật (sinh viên đối chiếu từng bullet với danh sách đồ án) |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | Chỉ chỉnh CV cho các JD đã được lọc phù hợp với thông tin (kỹ năng, dự án) hiện có của người dùng (tránh việc bịa CV để khớp với JD). AI không tự thêm kỹ năng, công nghệ hay số liệu không có trong dữ liệu đồ án; không tự nộp hồ sơ; chỉ dùng dữ liệu sinh viên cung cấp. Sinh viên bắt buộc đọc và duyệt từng dòng trước khi xuất PDF |

**Phản biện nhận được và đề xuất xử lý** (nhóm cần xác nhận lại ở cột cuối):

| Điểm yếu được chỉ ra | Nguồn | Đề xuất xử lý |
|---|---|---|
| Thời gian 45 phút/CV có thể do chưa có ngân hàng câu mô tả; template cố định có thể đã giảm thời gian mà không cần AI | AI phản biện trong bài cá nhân của Hiệu | Đưa "3 bản CV cố định + bullet bank" vào phương án No AI và đo song song (xem mục 6) |
| Rủi ro lớn nhất là AI tự bịa kỹ năng sinh viên không có để cố khớp với JD | AI phản biện trong bài cá nhân của Hiệu | Bổ sung bước AI lọc các JD phù hợp với thông tin (kỹ năng, dự án) hiện có ngay đầu quy trình; đặt boundary 100% khớp đồ án thật và bước duyệt từng dòng |
| Metric mới đo tốc độ, chưa đo chất lượng: CV nhanh hơn nhưng kém hơn thì sao? | Phản biện bổ sung (Claude) cho v0 | Thêm metric chất lượng ở v1 (tỉ lệ bullet phải sửa lại, số bullet sai sự thật) |
| Baseline chỉ là dữ liệu của 1 người (5 lần) | Phản biện bổ sung (Claude) cho v0 | Thu thêm số bấm giờ của ít nhất 2 người khác trước khi pilot |
| "100% khớp thực tế" chưa nói rõ cách đo | Phản biện bổ sung (Claude) cho v0 | Định nghĩa cách đo: mỗi bullet ghi đồ án nguồn, sinh viên tick xác nhận |

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **độ mơ hồ trung bình–cao, độ phức tạp thấp** → Workflow có AI ở 2 bước: lọc JD phù hợp với kỹ năng/dự án hiện có và nháp bullet mô tả đồ án (kèm Rule ở bước kiểm từ khóa và mẫu cố định).

Vì sao: đánh giá mức độ phù hợp ngữ cảnh giữa JD với dự án hiện có và viết lại bullet theo từng JD đều có độ mơ hồ trung bình–cao. Quy trình chỉ có 7 bước cố định, một người làm, hai nguồn dữ liệu là JD và hồ sơ thông tin hiện có (kỹ năng, danh sách đồ án) nên độ phức tạp thấp.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | 3 bản CV cố định (Java Backend, Node.js Backend, Fullstack) + ngân hàng câu mô tả đồ án trong Google Docs; mẫu CV có sẵn (ví dụ mẫu theo vị trí của TopCV) cho phần layout | JD khớp một trong các bản cố định, chỉ cần đổi vài dòng | Vẫn phải tinh chỉnh câu chữ khi JD lệch bản cố định; chưa có số đo thời gian cho phương án này | Giữ làm phương án so sánh và dùng khi đủ |
| **Rule** | Công cụ so khớp từ khóa JD với CV (như Match Report của Jobscan hoặc Teal bản free) để liệt kê từ khóa còn thiếu | Bước đọc JD và kiểm từ khóa | Không hiểu ngữ cảnh dự án để lọc JD sâu; không viết được câu; điểm match chỉ là ước lượng, dễ dẫn đến nhồi từ khóa | **Dùng cho bước kiểm từ khóa** |
| **Workflow** | **AI lọc các JD phù hợp với thông tin (kỹ năng, dự án) hiện có** → Rule kiểm từ khóa → sinh viên chọn đồ án → **AI nháp 3–5 bullet** từ dữ liệu đồ án thật và JD → sinh viên duyệt từng dòng → xuất PDF → sinh viên nộp | Các bước cố định (7 bước), AI hỗ trợ ở bước 1 (lọc JD chống bịa CV) và bước 4 (nháp ngôn ngữ bullet) | AI lọc nhầm hoặc nháp sai sự thật; sinh viên lười duyệt | **Chọn** |
| **Agent** | AI tự quét JD, tự chọn đồ án, tự sửa CV và tự nộp | Khi bước tiếp theo không đoán trước được | Nộp nhầm thông tin; bịa kỹ năng; khó kiểm soát | Không chọn |

**Mức chọn:** Workflow (có Rule ở bước kiểm từ khóa).

**Vì sao không chọn mức đơn giản hơn:** Đây là điểm nhóm chưa chứng minh được. Lập luận hiện có chỉ dựa trên phân tích của Hiệu: dù có bản cố định, bước tinh chỉnh câu chữ theo từng JD vẫn tốn thời gian, đúng phần mà No AI và Rule không viết được. Nhóm chưa có phỏng vấn thật hay số đo cho phương án No AI, và research ở mục 3.3 cho thấy bước này đã có công cụ hỗ trợ. Vì vậy mức Workflow được chọn **có điều kiện**: pilot phải đo song song No AI và Workflow trên các JD tương đương; nếu No AI đã đạt dưới 15 phút/CV thì quay về No AI.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | (1) Đánh giá và lọc ra các JD phù hợp với thông tin (kỹ năng, dự án) hiện có của người dùng (loại JD đòi kỹ năng không có để tránh bịa CV); (2) Bản nháp 3–5 bullet mô tả đồ án khớp JD, kèm từ khóa JD đã dùng và đồ án nguồn của từng bullet |
| **Judgment** — con người cân nhắc, quyết định gì? | Sinh viên quyết định đồ án nào nên nhấn cho JD đã lọc, từ khóa nào đáng đưa vào, và bullet nào đúng sự thật |
| **Action** — hành động cuối cùng là gì, ai làm? | Sinh viên sửa bullet, căn layout, xuất PDF và nộp |
| **Outcome** — đo kết quả bằng gì? | Thời gian chỉnh mỗi CV; tỉ lệ bullet phải sửa lại; số bullet có nội dung không có trong dữ liệu (mục tiêu 0); về lâu dài, tỉ lệ CV qua vòng hồ sơ |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Nội dung JD (có sẵn), thông tin hiện có của người dùng gồm danh sách kỹ năng và danh sách đồ án với vai trò, công nghệ, kết quả thật (cần tổng hợp một lần từ GitHub/README), CV gốc (có sẵn) |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Phần sinh viên sửa trong nháp mỗi lần; bullet bị xóa vì sai sự thật; các JD bị loại ở bước lọc; phản hồi của HR hoặc người review CV (nếu có) |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)?** **Augment.** Bằng chứng: phản biện của AI trong bài của Hiệu đề xuất agent tự nộp, và Hiệu không đồng ý vì rủi ro gửi nhầm thông tin; sinh viên muốn tự chọn đồ án và duyệt CV cuối. Đây mới là quan điểm của người đặt vấn đề.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót?** **Báo nhầm** (thêm kỹ năng hoặc số liệu không có để cố khớp với JD) tệ hơn: sinh viên có thể bị hỏi ngược lại trong phỏng vấn và mất uy tín. Bỏ sót chỉ làm bullet kém nổi bật hoặc thiếu từ khóa. Thiết kế xử lý: dùng AI lọc các JD phù hợp với thông tin (kỹ năng, dự án) hiện có ngay từ bước 1 để tránh cố ép CV theo JD lệch, AI chỉ dùng dữ liệu đồ án do sinh viên cung cấp, mỗi bullet ghi đồ án nguồn, sinh viên duyệt từng dòng và xóa mọi nội dung không nhớ đã làm.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên CNTT năm cuối ứng tuyển Fresher/Junior Backend/Fullstack, nộp nhiều đơn và chỉnh CV riêng cho từng JD |
| **Quy trình** | Lọc các JD phù hợp với thông tin (kỹ năng, dự án) hiện có → đọc JD và kiểm từ khóa → mở CV gốc và danh sách đồ án → chọn đồ án khớp JD → viết lại bullet mô tả đồ án → căn layout, xuất PDF → nộp và ghi Google Sheets |
| **Bottleneck** | Viết lại bullet mô tả đồ án theo từ khóa JD, khoảng 20 phút/CV (trên tổng 45 phút) |
| **Impact** | 45 phút/CV × 6 CV/tuần = 270 phút/tuần/sinh viên; có lúc nộp CV chung chung vì mệt |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian chỉnh một CV: 45' → dưới 15', sinh viên tự ghi giờ ≥ 5 CV trong 2 tuần pilot. (2) Sinh viên phải viết lại dưới 50% nháp AI. (3) 100% bullet có đồ án nguồn và được sinh viên xác nhận đúng sự thật. (4) Tỉ lệ qua vòng hồ sơ không thấp hơn 4 tuần trước pilot (chỉ theo dõi, khó đo chắc vì số đơn ít) |
| **Boundary** | Chỉ chỉnh CV cho các JD phù hợp với kỹ năng và dự án hiện có (tránh việc bịa CV để khớp với JD); AI không tự thêm kỹ năng, công nghệ hay số liệu không có trong danh sách đồ án; không tự nộp hồ sơ; chỉ dùng dữ liệu sinh viên cung cấp; sinh viên duyệt từng dòng trước khi xuất PDF |
| **AI intervention point** | (1) Bước 1: AI lọc các JD phù hợp với thông tin (kỹ năng, dự án) hiện có của người dùng để tránh bịa CV khớp JD; (2) Bước 4: Sau khi sinh viên đã chọn đồ án khớp JD và trước khi viết bullet |
| **Mức chọn** | Workflow (AI ở bước lọc JD và nháp bullet, kèm Rule ở bước kiểm từ khóa), có phương án đối chứng No AI |
| **Rủi ro & người kiểm tra** | AI bịa kỹ năng hoặc số liệu; nhồi từ khóa; duyệt qua loa. AI lọc bỏ JD lệch năng lực ngay ở bước 1; sinh viên đối chiếu từng bullet với danh sách đồ án ở bước 5; một thành viên khác trong nhóm đọc chéo 1 CV/tuần trong pilot |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Actor | Sinh viên CNTT năm cuối ứng tuyển Fresher/Junior | Thêm: nộp nhiều đơn và chỉnh CV riêng cho từng JD | Người dùng CV chung hoặc bản cố định có thể đã đủ với No AI. Tín hiệu này mới đến từ mục 3.2 và lập luận ở mục 6, cần xác nhận bằng phỏng vấn thật |
| Success Metric | Chỉ đo thời gian và 100% khớp thực tế | Thêm tỉ lệ viết lại nháp, số bullet có nguồn, theo dõi tỉ lệ qua vòng hồ sơ | Phản biện: CV nhanh hơn nhưng kém hơn thì không đạt |
| AI intervention point, Mức chọn, Rủi ro & người kiểm tra | Chưa có | Đã bổ sung | Hoàn tất sau khi chọn mức can thiệp ở mục 6 |

**Tiêu chí đánh giá đầu ra của AI (bản nháp bullet):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đúng sự thật | Mọi bullet truy được về một đồ án có thật trong danh sách; không có công nghệ hay số liệu lạ | Có kỹ năng, công nghệ hoặc số liệu không có trong danh sách đồ án |
| 2 | Khớp JD, không bỏ sót | Mọi từ khóa bắt buộc của JD mà sinh viên thực sự có đều xuất hiện trong nháp | Thiếu từ khóa bắt buộc mà sinh viên có trong đồ án |
| 3 | Không nhồi từ khóa | Mỗi bullet là một câu đọc tự nhiên, tối đa 2 dòng, có hành động và kết quả | Chỉ liệt kê từ khóa hoặc lặp từ khóa nhiều lần |
| 4 | Vai trò cá nhân rõ | Bullet nêu việc cụ thể của sinh viên trong đồ án | Chỉ nói chung chung "nhóm đã làm", không rõ phần của mình |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Trung bình | Bottleneck rõ ở bước viết bullet, nhưng bằng chứng thật mới là số bấm giờ của 1 người; chưa có phỏng vấn hay poll thật. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Trung bình | Chỉ cần sửa văn bản, không phải học công cụ mới. Nhưng phải chuẩn bị danh sách đồ án một lần, và có nguy cơ duyệt qua loa |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Thấp | Công cụ đã có (Teal, Jobscan, Kickresume hoặc prompt chuẩn); dữ liệu đồ án có sẵn trên GitHub; không cần xây gì |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Trung bình | Gói free có giới hạn (Teal giới hạn AI credits, Jobscan 5 lần quét, AI Writer của Kickresume ở gói trả phí). Đưa CV và dữ liệu cá nhân vào công cụ bên thứ ba cần xem điều khoản riêng tư. Sinh viên tự vận hành |

### 8.2. Kết luận

**Quyết định:** **Go, phạm vi nhỏ** (pilot 2 tuần, chưa xây gì).

**Lý do:** Không có rủi ro mức Cao. Feasibility thấp (công cụ có sẵn). Hai rủi ro Trung bình (Value, Viability) và Usability kiểm được ngay trong pilot, và pilot cũng chính là phép kiểm chứng đối chiếu với phương án No AI. Quyết định này dựa trên dữ liệu thật còn hạn chế (1 người bấm giờ, chưa có phỏng vấn thật), nên được coi là có điều kiện.

**Nếu Go — pilot nhỏ nhất (2 tuần):**

- Không xây gì. Mỗi người tham gia (Hiệu và ít nhất 2 thành viên khác) chỉnh ít nhất 5 CV cho các JD tương đương, luân phiên giữa hai cách: No AI (bản CV cố định + ngân hàng câu mô tả) và Workflow (Rule kiểm từ khóa + prompt chuẩn hoặc công cụ có gói free + sinh viên duyệt).
- Ghi giờ từng CV, ghi tỉ lệ nháp phải viết lại, chấm nháp theo 4 tiêu chí ở mục 7.
- Trước pilot: thu thêm số bấm giờ baseline của ít nhất 2 người; phỏng vấn thật 2–3 sinh viên năm cuối ngoài nhóm theo The Mom Test và poll 5–10 người; đọc điều khoản riêng tư của công cụ định dùng.

**Nếu Not Yet — cần kiểm chứng gì trước:** Không áp dụng cho quyết định hiện tại. Nếu phỏng vấn thật phản bác bottleneck (đa số dùng CV chung hoặc mất dưới 15 phút), chuyển sang Not Yet và kiểm chứng lại actor.

**Nếu No-Go — nên làm gì thay AI:** Dùng bản CV cố định theo hướng Java Backend, Node.js Backend, Fullstack + ngân hàng câu mô tả đồ án + mẫu CV có sẵn.

**Ngưỡng dừng:**

- Nếu No AI đạt dưới 15 phút/CV (trung vị ≥ 5 CV) → quay về No AI, không dùng AI.
- Nếu 2 CV liên tiếp phải viết lại trên 50% bản nháp → dừng Workflow, quay về No AI.
- Nếu có 1 bullet sai sự thật mà sinh viên không phát hiện trước khi nộp → dừng pilot, xem lại bước duyệt.
- Nếu công cụ không rõ về dữ liệu cá nhân hoặc buộc trả phí để dùng được → không dùng công cụ đó, thử prompt chuẩn hoặc quay về No AI.

---

## 9. Hạn chế và hướng tiếp theo

- Bằng chứng thật còn mỏng: baseline 45 phút/CV chỉ từ 5 lần bấm giờ của 1 người (Hiệu). Chưa có phỏng vấn thật và chưa có poll.
- Điểm chấm shortlist ở CP3, điểm trong Assumption Map và các số phút của quy trình tương lai là ước lượng, chưa đo.
- Nhóm chưa tự dùng thử các công cụ ở mục 3.3; thông tin lấy từ trang chính thức và bài đánh giá bên thứ ba, giá và tính năng có thể đổi.
- Chưa đo được chất lượng CV theo nghĩa "qua vòng hồ sơ", vì số đơn ít và nhà tuyển dụng ít phản hồi.
- Hướng tiếp theo: các candidate cùng chuỗi ứng tuyển (đọc và lọc JD, chuẩn bị phỏng vấn) cho vòng sau; bài "phân loại ca lỗi production" chỉ xét lại nếu nhóm có quyền tiếp cận dữ liệu thật.

## 10. Tài liệu tham khảo

Ngày kiểm tra các link: 09/11/2026.

- Teal AI Resume Builder: https://www.tealhq.com/free và https://tealhq.com/resume-builder
- Jobscan Match Report: https://jobscan.co/resume-matcher và https://www.jobscan.co/resume-checker
- Kickresume (AI Writer, giá): https://www.kickresume.com/pricing
- TopCV, tạo CV online theo mẫu: https://www.topcv.vn/cach-tao-cv-online-tren-topcv
- Hướng dẫn dùng AI viết CV (tiếng Việt, blog): https://findskill.ai/vi/blog/ai-viet-cv-xin-viec-2026-huong-dan-tieng-viet/
- Rezi, bài tổng hợp công cụ viết CV (blog của nhà bán công cụ): https://www.rezi.ai/posts/rezi-alternatives
- Rob Fitzpatrick, *The Mom Test* (3 luật phỏng vấn dùng ở mục 3.2)
- Google PAIR, *People + AI Guidebook* (hai câu hỏi augment/automate và báo nhầm/bỏ sót ở mục 6.4)
- Các bài cá nhân của Nhân, Hải Anh, Hiệu, Dũng; `CHECKPOINTS.md` và bài mẫu của môn học
