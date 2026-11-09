# Báo cáo cá nhân — 2A202604037_TranAnhDung

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Anh Dũng
- MSSV:2A202604037
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:FreeFire
- Link repo nhóm:https://github.com/nhan54v-boop/K5-L3B-Day02-FreeFire-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

**Bối cảnh nhân vật:** Nam, AI Engineer tại một công ty sản phẩm công nghệ (team AI & Data khoảng 15 người), phụ trách phát triển và vận hành các dịch vụ Computer Vision và RAG/LLM trên môi trường production. Công cụ sử dụng hàng ngày: GitLab (code & CI/CD), cụm máy chủ GPU Linux/Docker, MLflow/WandB, hệ thống giám sát log (Grafana/ELK), Jira và Slack.

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi chuẩn bị release model mới vào thứ Năm hàng tuần, tôi muốn có bản so sánh benchmark (accuracy, latency, VRAM) với bản prod và phát hiện regression, để gửi Tech Lead và PM duyệt go-live trước 15h. | AI Engineer, Tech Lead, Product Manager | Bấm giờ 2 đợt gần nhất: mất 80–95 phút để gom số liệu từ MLflow, script benchmark và viết đánh giá. |
| 2 | Lặp lại | Khi kết thúc sprint 2 tuần, tôi muốn gom nhanh chi phí cloud GPU, token API và danh sách container lãng phí về một bảng, để báo cáo tối ưu hạ tầng cho Engineering Manager. | AI Engineer, DevOps, Engineering Manager | Mất ~45 phút mỗi cuối sprint để xuất billing từ 3 dịch vụ và đối chiếu với danh sách job của team. |
| 3 | Tốn thời gian | Khi nhận 100–200 ca đoán sai (bad cases) từ production mỗi tuần, tôi muốn phân loại nhanh nguyên nhân (nhiễu input, data drift hay hậu xử lý), để quyết định chiến lược lấy data retrain. | AI Engineer, Đội QA, Annotators | ~2 tiếng/tuần mở từng mẫu lỗi, đối chiếu log JSON vào Google Sheets; tuần trước tồn đọng 80 ca chưa xem. |
| 4 | Tốn thời gian | Khi tích hợp model mới từ paper vào codebase công ty, tôi muốn phát hiện sớm xung đột thư viện (CUDA, TensorRT, PyTorch) và chuẩn hóa I/O, để đóng gói Docker chạy test không lỗi môi trường. | AI Engineer, MLOps | Mất 3–4 tiếng/lần tích hợp chỉ để gỡ lỗi môi trường và sửa script chuyển đổi trọng số. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi AI API trên production bị spike latency hoặc trả lỗi hàng loạt, tôi muốn đối chiếu ngay traceback log, tải GPU và commits gần nhất, để khoanh vùng nguyên nhân và xử lý sự cố trong 15 phút. | AI Engineer trực on-call, Backend Dev, End-user | Mất 30–45 phút/sự cố mở 4 tab (Grafana, Docker logs, GitLab, Slack); tháng trước có 3 lần vượt SLA. |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi thiết kế giải pháp AI cho tính năng mới từ PRD, tôi muốn tra cứu lại kết quả thực nghiệm cũ, giới hạn phần cứng và kiến trúc trước đây, để viết Technical Design Doc khả thi. | AI Engineer, Tech Lead, PM | ~2 tiếng/lần viết Design Doc vì thông tin rải rác ở Notion, GitLab Wiki và Slack cũ; tần suất 1–2 lần/tháng. |
| 7 | Pain từ người khác | Khi Backend tích hợp hoặc cập nhật AI API vào hệ thống chính, họ muốn tài liệu đặc tả luôn khớp với code kèm ví dụ payload/mã lỗi, để không bị lỗi lệch kiểu dữ liệu khi gọi hàm. | Backend Dev, Mobile Dev, AI Engineer | Backend nhắn hỏi lại 4–6 lần/đợt cập nhật do Swagger/Notion chưa đồng bộ code; mất ~40 phút hỗ trợ/đợt. |
| 8 | Pain từ người khác | Khi PM hoặc khách hàng hỏi lý do hệ thống AI dự đoán bất thường ở ca cụ thể, họ muốn có giải thích bằng ngôn ngữ nghiệp vụ thay vì bảng log, để phản hồi kịp thời cho đối tác. | Product Manager, CSKH, Khách hàng, AI Engineer | Mất 20–25 phút/ca để dịch log confidence score sang giải thích nghiệp vụ; trung bình 5–6 ca/tuần. |
| 9 | Tốn thời gian | Khi chuẩn bị golden test set cho pipeline RAG/LLM, tôi muốn rà soát và làm sạch các cặp Q&A chuẩn từ tài liệu nghiệp vụ mới cập nhật, để bộ đánh giá tự động không bị chấm sai theo thông tin cũ. | AI Engineer, Domain Expert | Mất ~2,5 tiếng mỗi khi công ty cập nhật quy định/sản phẩm mới để đối chiếu và sửa lại 150 câu test mẫu. |
| 10 | Lặp lại | Khi review Merge Request của Junior/Intern hàng ngày, tôi muốn kiểm tra nhanh chuẩn quản lý VRAM GPU, biến cấu hình và kết quả test, để góp ý trọng tâm mà không bỏ sót lỗi cơ bản. | AI Engineer (Reviewer), Junior/Intern AI | 25–30 phút/MR, trung bình 4–5 MR/tuần; tuần trước sót 1 MR quên giải phóng VRAM làm treo worker sau 12h. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại:** Ý #9 (Rà soát golden test set cho pipeline RAG) và #10 (Pre-check MR của Junior/Intern về chuẩn VRAM) — vì có quy trình lặp lại cụ thể, dễ đo lường thời gian thực tế và là bottleneck thường trực trong team AI.
- **Ý bỏ:** Ý AI đề xuất về *"Trợ lý AI tự động tối ưu hóa toàn bộ pipeline model và kiến trúc từ A-Z"* — vì phạm vi quá rộng, thiếu ranh giới giải pháp cụ thể và không bám vào một quy trình nghiệp vụ thực tế.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|:---:|---|---|---|
| 1 | Phân loại ca lỗi thực tế — Production Bad Cases Triage (#3) | Quy trình rõ ràng, ngốn 2 tiếng/tuần lặp lại, có dữ liệu log thực tế để đo baseline, dễ so sánh 4 mức can thiệp | Tiêu chí phân nhóm lỗi của AI thế nào là "đủ chính xác" để quyết định hướng retrain? |
| 2 | Đồng bộ tài liệu đặc tả API/Model cho Backend (#7) | Pain thật từ đồng nghiệp (Backend hỏi lại 4–6 lần/đợt), giảm thời gian gián đoạn công việc | Dùng công cụ tự sinh doc từ code (Rule/FastAPI) đã đủ chưa hay thực sự cần tới AI? |
| 3 | Báo cáo chi phí GPU/API & tiến trình lãng phí cuối sprint (#2) | Tác động trực tiếp đến chi phí hạ tầng của team, có số liệu định lượng rõ | Phần lớn bước là cộng trừ số liệu và dò log hệ thống, liệu Rule/Script đã giải quyết được 90% chưa? |

---

### Problem Card #1 — Phân loại ca lỗi thực tế (Production Bad Cases Triage - #3)

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi nhận được danh sách 100–200 ca dự đoán sai từ môi trường thực tế (production bad cases) do đội QA và CSKH chuyển về mỗi tuần, tôi muốn phân loại nhanh nguyên nhân (do nhiễu dữ liệu đầu vào, lệch phân phối hay lỗi hậu xử lý), để quyết định chiến lược lấy thêm dữ liệu retrain |
| **Actor** | AI Engineer phụ trách duy trì chất lượng mô hình trên production (phối hợp với QA và đội gán nhãn) |
| **Thời điểm / bối cảnh** | Sáng thứ Ba hằng tuần, trước buổi họp chốt kế hoạch thu thập và gán nhãn dữ liệu bổ sung lúc 14h |
| **Quy trình hiện tại** | 1. Tải danh sách ticket báo lỗi từ Jira/Sheets của QA · 2. Truy xuất request ID trong ELK/S3 để lấy ảnh/text gốc và JSON output của model · 3. Mở xem từng mẫu, đối chiếu confidence score và đầu vào · 4. Gắn nhãn nguyên nhân lỗi (nhiễu đầu vào, out-of-distribution, lỗi rule hậu xử lý, nhãn gốc sai) · 5. Gom nhóm các pattern lỗi lặp lại và viết nhận định ưu tiên cần xử lý · 6. Tạo task yêu cầu đội Data Annotators lấy thêm dữ liệu theo nhóm lỗi · 7. Gửi báo cáo tổng hợp trên Slack |
| **Bottleneck** | Bước 3 & 5: Xem thủ công từng mẫu kết hợp đọc log và viết nhận định gom nhóm pattern lỗi (mất khoảng 75 phút/120 phút tổng cộng) |
| **Impact** | ~120 phút/tuần cho 1 AI Engineer; team có 3 dịch vụ AI nên tốn ~360 phút/tuần; tuần trước tồn đọng 80 ca không kịp phân tích làm trễ 1 đợt retrain |
| **Success metric** | Giảm tổng thời gian từ 120 phút xuống dưới 35 phút/tuần; tỷ lệ AI Engineer phải sửa lại nhãn phân loại nháp dưới 20%; không bỏ sót nhóm lỗi nghiêm trọng (critical failure mode) nào |
| **Phương án không dùng AI** | Yêu cầu QA điền form phân loại sẵn + viết Python script tự động gom nhóm theo ngưỡng confidence score và kích thước/độ dài input: giúp lọc nhanh lỗi kỹ thuật, nhưng không tự đọc hiểu được ngữ cảnh lỗi ngữ nghĩa hoặc mô tả phàn nàn tự do của khách |
| **Giả thuyết về AI** | Dùng script (Rule) tự động gom log + ảnh/text gốc, sau đó dùng AI (VLM/LLM) đọc phản hồi của QA + output model để gợi ý nhãn nguyên nhân và tóm tắt các cụm lỗi phổ biến; AI Engineer chỉ duyệt lại và chốt hướng retrain |
| **Cảm nhận nhanh** | Workflow |

**Quy trình nháp (Card #1):**

```text
HIỆN TẠI — 120 phút/tuần

[1 Lấy danh sách ticket QA: 10'] → [2 Truy xuất log JSON & dữ liệu gốc: 20'] 
→ [3 Xem mẫu & đối chiếu output: 45'] ← BOTTLENECK
→ [4 Gắn nhãn nguyên nhân từng ca: 15'] → [5 Gom pattern & viết nhận định: 15'] ← BOTTLENECK
→ [6 Tạo yêu cầu cho đội gán nhãn: 10'] → [7 Gửi báo cáo Slack: 5']
```

---

### Problem Card #2 — Đồng bộ tài liệu đặc tả API/Model cho Backend (#7)

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi Backend tích hợp hoặc cập nhật AI API vào hệ thống chính, họ muốn tài liệu đặc tả luôn khớp với code kèm ví dụ payload/mã lỗi, để không bị lỗi lệch kiểu dữ liệu khi gọi hàm và không phải hỏi lại. |
| **Actor** | AI Engineer & Backend Dev |
| **Thời điểm / bối cảnh** | Mỗi đợt release/cập nhật model hoặc thay đổi API endpoint |
| **Quy trình hiện tại** | 1. Sửa code/schema: 5' · 2. Chạy test payload: 10' · 3. Viết/cập nhật bảng mô tả trường dữ liệu, ngưỡng threshold & mã lỗi lên Notion: 20' · 4. Gửi link & giải thích lại trên Slack: 25' |
| **Bottleneck** | Bước 3 & 4: Viết mô tả ngữ nghĩa cho các tham số model và trả lời tin nhắn hỏi lại trên Slack (mất ~45 phút / tổng 60 phút) |
| **Impact** | Backend hỏi lại 4–6 lần/đợt do Swagger/Notion chưa đồng bộ code; gián đoạn công việc của cả hai bên; mất ~60 phút hỗ trợ/đợt release |
| **Success metric** | Giảm thời gian viết & giải thích từ 60 phút xuống dưới 15 phút/đợt release; số lần Backend hỏi lại trên Slack từ 4–6 lần xuống ≤ 1 lần/đợt |
| **Phương án không dùng AI** | Dùng công cụ tự sinh OpenAPI/Swagger doc từ code (FastAPI/Pydantic): sinh được schema kỹ thuật nhưng thiếu giải thích ngữ nghĩa, ngưỡng threshold nghiệp vụ và ví dụ payload thực tế |
| **Giả thuyết về AI** | Dùng script sinh schema kết hợp AI (LLM) đọc docstring/code để tự động sinh mô tả tham số và ví dụ gọi API sát thực tế; AI Engineer duyệt nhanh trước khi publish |
| **Cảm nhận nhanh** | Rule kết hợp Workflow |

**Quy trình nháp (Card #2):**

```text
HIỆN TẠI — 60 phút/đợt release

[1 Sửa code/schema: 5'] → [2 Chạy test payload: 10']
→ [3 Viết/cập nhật bảng mô tả trường dữ liệu, threshold & mã lỗi lên Notion: 20'] ← BOTTLENECK
→ [4 Gửi link & giải thích lại trên Slack: 25'] ← BOTTLENECK
```

---

### Problem Card #3 — Báo cáo chi phí GPU/API & tiến trình lãng phí cuối sprint (#2)

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi kết thúc sprint 2 tuần, tôi muốn gom nhanh chi phí cloud GPU, token API và danh sách container/tiến trình treo lãng phí về một bảng, để báo cáo tối ưu hạ tầng cho Engineering Manager. |
| **Actor** | AI Engineer & Engineering Manager |
| **Thời điểm / bối cảnh** | Cuối sprint 2 tuần (thứ Sáu trước buổi sprint review) |
| **Quy trình hiện tại** | 1. Xuất CSV chi phí Cloud/API: 10' · 2. SSH kiểm tra log nvidia-smi & docker stats: 15' · 3. Đối chiếu từng container với chủ nhân & tính thời gian treo lãng phí: 15' · 4. Viết đề xuất tắt/giảm cấu hình: 5' |
| **Bottleneck** | Bước 3: Khớp nối danh sách tiến trình treo với lịch sử chạy job của các thành viên (mất 15 phút / tổng 45 phút) |
| **Impact** | Mất ~45 phút mỗi cuối sprint để xuất billing từ 3 dịch vụ và đối chiếu; nguy cơ lãng phí ngân sách GPU idle kéo dài |
| **Success metric** | Giảm thời gian làm báo cáo từ 45 phút xuống dưới 10 phút/sprint; phát hiện 100% container treo quá 12 tiếng không dùng GPU |
| **Phương án không dùng AI** | Viết cronjob bash script định kỳ quét nvidia-smi và gửi cảnh báo container có GPU utilization = 0% quá 12h vào Slack |
| **Giả thuyết về AI** | Script Rule-based tự động gom log và số liệu; AI (LLM) tóm tắt biến động chi phí so với sprint trước và gợi ý phương án tối ưu tài nguyên; Manager review |
| **Cảm nhận nhanh** | Rule (Script định kỳ) hoặc Workflow đơn giản |

**Quy trình nháp (Card #3):**

```text
HIỆN TẠI — 45 phút/sprint

[1 Xuất CSV chi phí Cloud/API: 10'] → [2 SSH kiểm tra log nvidia-smi & docker stats: 15']
→ [3 Đối chiếu từng container với chủ nhân & tính thời gian treo lãng phí: 15'] ← BOTTLENECK
→ [4 Viết đề xuất tắt/giảm cấu hình: 5']
```

---

### Card #2 và #3 (Tóm tắt)

| Card | Actor | Quy trình nháp & Bottleneck | Metric | Cảm nhận nhanh |
| --- | --- | --- | --- | --- |
| **#2 Đồng bộ tài liệu API/Model Spec cho Backend (#7)** | AI Engineer & Backend Dev | `[1 Sửa code/schema: 5']` → `[2 Chạy test payload: 10']` → **`[3 Viết/cập nhật bảng mô tả trường dữ liệu, ngưỡng threshold & mã lỗi lên Notion: 20' - BOTTLENECK]`** → `[4 Gửi link & giải thích lại trên Slack: 25']`<br><br>• **Nghẽn:** Bước 3 & 4 (viết mô tả ngữ nghĩa cho các tham số model và trả lời tin nhắn hỏi lại) | Giảm thời gian viết & giải thích từ 60 phút xuống dưới 15 phút/đợt release; số lần Backend hỏi lại trên Slack từ 4–6 lần xuống $\le 1$ lần/đợt | Rule kết hợp Workflow |
| **#3 Báo cáo chi phí GPU/API & tiến trình lãng phí (#2)** | AI Engineer & Engineering Manager | `[1 Xuất CSV chi phí Cloud/API: 10']` → `[2 SSH kiểm tra log nvidia-smi & docker stats: 15']` → **`[3 Đối chiếu từng container với chủ nhân & tính thời gian treo lãng phí: 15' - BOTTLENECK]`** → `[4 Viết đề xuất tắt/giảm cấu hình: 5']`<br><br>• **Nghẽn:** Bước 3 (khớp nối danh sách tiến trình treo với lịch sử chạy job của các thành viên) | Giảm thời gian làm báo cáo từ 45 phút xuống dưới 10 phút/sprint; phát hiện 100% container treo quá 12 tiếng không dùng GPU | Rule (Script định kỳ) hoặc Workflow đơn giản |

---

### Card muốn pitch nhất

- Card số: Card #1 (Từ Problem #3 — Phân loại ca lỗi thực tế / Production Bad Cases Triage)
- Vì sao: Quy trình rõ ràng 7 bước, ngốn 120 phút/tuần lặp lại, có dữ liệu log thực tế để đo baseline (120' xuống < 35'), điểm nghẽn nằm đúng ở phần đọc hiểu/tổng hợp ngữ cảnh rất hợp để phân tích sâu chuỗi Rule → AI Workflow → Con người duyệt (Human-in-the-loop).
- Câu hỏi muốn nhóm phản biện: "Tiêu chí phân nhóm lỗi của AI thế nào là 'đủ chính xác' để quyết định hướng retrain, và làm sao tránh rủi ro 'mù kép' khi dùng mô hình AI để bắt lỗi của một mô hình AI khác?"

---

### Bản Pitch nhanh (Dùng để trình bày nhóm ở CP3)

```text
┌──────────────────────────────────────────────────────────────────────────┐
│ PROBLEM CARD #1 (Từ Problem #3 — Phân loại ca lỗi thực tế)               │
│ Khi nhận 100–200 ca dự đoán sai từ thực tế mỗi tuần, tôi muốn phân loại  │
│ nhanh nguyên nhân gốc, để quyết định chiến lược lấy dữ liệu retrain.     │
│ Ai chịu ảnh hưởng? AI Engineer, QA, Đội gán nhãn (Annotators)            │
│ Quy trình: 1.Lấy ticket → 2.Kéo log/ảnh → 3.Xem & đối chiếu →            │
│            4.Gắn nhãn lỗi → 5.Gom pattern & nhận định → 6.Giao task      │
│ Bước nghẽn: Xem mẫu + gom pattern viết nhận định (75 phút/lần)           │
│ Đo thành công: từ 120 phút xuống < 35 phút/tuần (tỷ lệ sửa lại < 20%)    │
│ Cảm nhận nhanh: □ No AI  □ Rule  ■ Workflow  □ Agent  □ Chưa biết        │
└──────────────────────────────────────────────────────────────────────────┘
```

---

### AI phản biện Card #1 (Production Bad Cases Triage)

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
| --- | --- | --- |
| **Baseline 120 phút mới là ước lượng chủ quan**, chưa tách rõ thời gian chờ tải dữ liệu và thời gian đọc phân tích thật sự | Đồng ý | Đo lại bằng cách bấm giờ thực tế trên 2 batch gần nhất (115 phút và 130 phút); tách riêng bước kéo log (20 phút) và bước đọc/gom nhóm (75 phút) |
| **Bước 2 (truy xuất log) và một phần bước 4 có thể giải quyết hoàn toàn bằng Python script (Rule)** mà chưa cần tới AI | Đồng ý | Cập nhật lại giả thuyết: Dùng script tự động kéo dữ liệu và lọc trước các lỗi kỹ thuật rõ ràng (ảnh mờ/rỗng, timeout); chỉ dùng AI ở bước gom cụm ngữ nghĩa và tóm tắt mô tả lỗi của QA |
| **Dùng mô hình AI để bắt lỗi của một mô hình AI khác dễ gặp rủi ro "mù kép"** (cả 2 cùng sai trên một kiểu dữ liệu khó) | Đồng ý một phần | Không để AI tự động xóa ca lỗi hay tự động đưa vào tập train; giữ boundary bắt buộc là **AI Engineer phải duyệt lại các cụm lỗi** trước khi giao task cho đội gán nhãn |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
