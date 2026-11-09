# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm:
- Candidate problem nhóm chọn (1 câu):
- Quyết định cuối (Go / Not Yet / No-Go):

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | Trần Anh Dũng | 2A202604037 | ghi chép, người phản biện chính | tad-4963 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | | | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | | | Assumption map, snapshot hoặc survey |
| CP4 — Research | | | Bảng research có link |
| CP5 — Quy trình trước/sau | | | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | | | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | | | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | | | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### TranAnhDung-2A202604037

**Phần việc phụ trách:**

- Xây dựng bộ slide trình chiếu và thuyết trình tương tác của nhóm.
- Phản biện phương án giải quyết, đóng góp hoàn thiện quy trình tương lai CP5 (bổ sung bước AI lọc JD phù hợp để tránh bịa CV) và mức can thiệp AI CP6.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Hoàn thành báo cáo cá nhân: scan 10 problem cards, đề xuất Candidate #10 (Phân loại ca lỗi production) và tham gia pitch, thảo luận hội tụ nhóm ở CP3.
- Trực tiếp lập trình và hoàn thiện toàn bộ file slide thuyết trình với giao diện hiện đại, responsive, trực quan hóa toàn bộ hành trình CP4–CP6 và quy trình Trước/Sau phục vụ thuyết trình 6 phút.
- Cập nhật quy trình tương lai trong: đưa bước AI lọc các JD phù hợp với năng lực hiện có ngay từ đầu, chuẩn hóa quy trình thành 7 bước nhằm triệt tiêu nguy cơ sinh viên/AI cố tình bịa CV để khớp với JD lệch.

**Bằng chứng** :

- Báo cáo cá nhân: `report/individual/2A202604037_TranAnhDung.md` .
- File slide thuyết trình: `report/team/slides.html` .
  - Mục 2.1 , Mục 2.4 .
  - Mục 3.2 .
  - Mục 4.2, 4.3 và Mục 5, 6, 7.

**Điều mình học được từ phần nhóm:**

- Nhận thức rõ ràng về việc chọn bài toán: Không phải bài toán nào phức tạp về mặt kỹ thuật cũng là bài toán tối ưu để làm; bài toán tốt cần có actor cụ thể, bottleneck đo đếm được bằng thời gian thực tế và vừa sức để kiểm chứng, giải quyết triệt để trong khuôn khổ lab.
- Thấu hiểu nguyên tắc "No AI / Rule First": Nhận ra rằng nếu 2–3 bản CV cố định kết hợp Bullet Bank đã giải quyết tốt 80% trường hợp thì AI chỉ nên đóng vai trò augment ở đúng bước nghẽn ngôn ngữ (soạn nháp bullet và lọc JD), không nên lạm dụng công cụ hay nhảy vội sang Agent tự động hóa hoàn toàn.
- Tầm quan trọng của ranh giới (Boundary) và cơ chế Human-in-the-loop (HITL): Với AI tạo sinh trong CV, lỗi "báo nhầm" (bịa đặt thông tin) là tối kỵ vì đánh mất uy tín ứng viên. Việc thiết kế cổng lọc JD phù hợp ngay từ đầu và duy trì con người kiểm duyệt từng dòng là bắt buộc để đảm bảo hồ sơ luôn đúng sự thật 100%.
