# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: xyz
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Sinh viên gặp khó khăn và mất nhiều thời gian (3–5 giờ/môn) để tự tổng hợp, hệ thống hóa kiến thức cốt lõi và công thức chính xác kèm trang nguồn đối chiếu từ các bộ slide/giáo trình dài (200+ trang) hoặc mới cập nhật khi chưa có đề cương khóa trước đáng tin cậy.
- Quyết định cuối: **Go (Phạm vi nhỏ — Triển khai Pilot quy trình Workflow bán thủ công trên công cụ có sẵn, có bước con người kiểm chứng công thức)**

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Phạm Quỳnh Anh | Khi khách hàng nhắn tin hỏi thông tin sản phẩm (giá, kích thước, tình trạng còn hàng) ngoài giờ hành chính (22h–7h), tôi muốn cung cấp thông tin chính xác và tư vấn tức thì cho khách, để giữ chân khách mua hàng mà tôi không phải thức đêm trực page. | Chủ cửa hàng online, nhân viên trực page, khách mua ban đêm | Độ trễ phản hồi qua đêm 6–8 tiếng khiến khách chuyển sang shop khác (tỷ lệ rớt đơn ban đêm 40%). | "Nếu khách chỉ hỏi dạo lúc 2h sáng rồi không mua thì có tốn công không? Giải pháp Rule tự động gửi tin nhắn mẫu có sẵn của Facebook có giải quyết được không?" (Vũ Đức Minh hỏi) |
| 2 | Phạm Quỳnh Anh | Khi phát sinh các khoản chi tiêu nhỏ lẻ trong ngày (tiền ăn, gửi xe, tiền mua đồ), tôi muốn ghi nhận lại số tiền và phân loại vào các khoản mục, để kiểm soát chi tiêu hàng tháng mà không phải nhớ lại và cộng trừ lại vào cuối ngày. | Cá nhân, sinh viên | Bước nhớ lại và gõ tay từng dòng vào Excel/app mỗi tối (15–20 phút), dễ bỏ cuộc sau 1 tuần. | "Tại sao không dùng app như Money Lover hay kiểm tra lịch sử biến động số dư ngân hàng? Rào cản lớn nhất là do bạn lười nhập liệu hay do app hiện tại khó dùng?" (Nguyễn Văn Nhi hỏi) |
| 3 | Phạm Quỳnh Anh | Khi ôn thi cuối kỳ với hơn 200 trang slide bài giảng, tôi muốn trích xuất các công thức và kiến thức cốt lõi thành bản tóm tắt, để có thể ghi nhớ nhanh chóng mà không mất 4–5 tiếng lật giở từng trang slide. | Sinh viên đại học | Bước đọc lướt và gõ lại công thức/định nghĩa sang file Word (mất 4–5 tiếng/môn). | "Dữ liệu slide bài giảng có nhiều hình vẽ, công thức toán dạng ảnh chụp và không có cấu trúc cố định thì hệ thống có đọc được không? Đã thử xin tóm tắt của khóa trên chưa?" (Vũ Đức Minh hỏi) |
| 4 | Vũ Đức Minh | Khi một nhân viên mới bắt đầu làm việc, tôi muốn được cấp đầy đủ tài khoản và quyền truy cập vào các hệ thống cần thiết theo vị trí công việc, để có thể bắt đầu thực hiện nhiệm vụ mà không phải chờ đợi các bộ phận liên quan thiết lập tài khoản. | Nhân viên mới, HR, IT/System Admin, quản lý trực tiếp | Bước xác định hệ thống cần cấp quyền, gửi yêu cầu, chờ phê duyệt từ nhiều đầu mối và thiết lập tài khoản trên từng hệ thống (mất vài ngày). | "Việc cấp quyền truy cập hệ thống công ty có chính sách bảo mật nghiêm ngặt và cần người chịu trách nhiệm, liệu có rủi ro bảo mật nào nếu tự động hóa khâu phân quyền này không?" (Phạm Quỳnh Anh hỏi) |
| 5 | Vũ Đức Minh | Khi người dân đến hỏi về một thủ tục hành chính, tôi muốn xác định đầy đủ hoàn cảnh và điều kiện của họ để hướng dẫn chính xác các giấy tờ, bước thực hiện cần thiết, nhằm hạn chế việc người dân phải đi lại nhiều lần do thiếu hồ sơ. | Cán bộ tiếp nhận hồ sơ, cán bộ tư vấn, người dân, cơ quan hành chính | Cán bộ phải khai thác thông tin, tra cứu quy định và đối chiếu điều kiện; cán bộ ít kinh nghiệm dễ bỏ sót câu hỏi hoặc trường hợp ngoại lệ. | "Quy định pháp luật và thủ tục hành chính thay đổi thường xuyên theo thông tư mới, làm sao đảm bảo thông tin tra cứu luôn được cập nhật chính xác và có giá trị pháp lý?" (Nguyễn Văn Nhi hỏi) |
| 6 | Vũ Đức Minh | Khi nhận được đơn đặt hàng cho mặt hàng công ty không còn tồn kho, tôi muốn nhanh chóng tìm được các nhà cung cấp thay thế có hàng sẵn, giá nhập và thời gian giao phù hợp, để đáp ứng đơn hàng và hạn chế mất doanh thu. | Nhân viên kinh doanh, nhân viên mua hàng, nhà cung cấp, khách hàng | Tìm kiếm và liên hệ nhiều nhà cung cấp, chờ phản hồi rồi tổng hợp thông tin so sánh giá và thời gian giao. | "Các nhà cung cấp bên ngoài thường không công khai tồn kho real-time qua API, vậy làm sao thu thập được dữ liệu tồn kho của họ mà không phải gọi điện thoại hỏi tay?" (Phạm Quỳnh Anh hỏi) |
| 7 | Nguyễn Văn Nhi | Khi bắt đầu thực hiện một bài tập Lab, tôi muốn nhanh chóng xác định được các yêu cầu, hướng dẫn thực hiện và quy định nộp bài từ những tài liệu liên quan, để hiểu đúng nhiệm vụ và bắt đầu triển khai mà không mất quá nhiều thời gian tìm kiếm thông tin. | Học viên thực hiện bài Lab (cá nhân và nhóm), Mentor hỗ trợ | Dò tìm và đối chiếu chéo yêu cầu/rule/rubric giữa 5–6 file tài liệu rời rạc (`Slide`, `README`, `RULES`, `CHECKPOINTS`, `RUBRIC`) mất 15–20 phút/lần. | "Tại sao không chỉ cần ban tổ chức gộp các yêu cầu thành 1 bảng checklist duy nhất ngay đầu file CHECKPOINTS (No AI/Rule) thay vì phải xây dựng giải pháp công nghệ phức tạp?" (Vũ Đức Minh hỏi) |
| 8 | Nguyễn Văn Nhi | Khi viết báo cáo nghiên cứu khoa học hoặc luận văn, tôi muốn đảm bảo mỗi nội dung, số liệu và nhận định trong bài viết đều được đối chiếu chính xác với nguồn tài liệu gốc, đồng thời duy trì đúng thứ tự trích dẫn, để tránh sai lệch thông tin và đáp ứng yêu cầu học thuật. | Sinh viên làm khóa luận/NCKH, Giảng viên hướng dẫn, Người phản biện | Mở lại từng paper PDF gốc để đối chiếu thủ công độ khớp giữa nhận định/số liệu trong bài viết với nội dung bài báo gốc (mất 25 phút/lần rà soát chương). | "Đã có các phần mềm quản lý trích dẫn như Zotero hay BibTeX giải quyết việc đánh số và định dạng, việc kiểm tra độ khớp ngữ nghĩa giữa câu viết và paper gốc có thực sự làm được bằng AI với chi phí token hợp lý không?" (Phạm Quỳnh Anh hỏi) |
| 9 | Nguyễn Văn Nhi | Khi thực hiện các thí nghiệm Ablation trong quá trình nghiên cứu, tôi muốn xác định chính xác cấu hình mô hình, phiên bản dữ liệu và các thay đổi được áp dụng cho từng lần chạy, để có thể truy vết, đối chiếu và sử dụng đúng kết quả thực nghiệm khi phân tích và viết luận văn. | Sinh viên/NCS làm Machine Learning, Thành viên nhóm nghiên cứu | Dò tìm lại cấu hình từ các file log rời rạc (30 phút) và phải chạy lại thí nghiệm khi không truy vết được (mất 4–6 tiếng GPU/lần chạy). | "Vấn đề này đã có các công cụ MLOps chuyên dụng như Weights & Biases (W&B) hoặc MLflow giải quyết rất tốt bằng việc lưu log tự động, liệu có cần can thiệp AI vào đây không hay chỉ là vấn đề kỷ luật dùng công cụ?" (Vũ Đức Minh hỏi) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung (Bản chất công việc) |
|---|---|---|
| **A — Hỗ trợ và khai thác thông tin** | `#1` Trả lời khách hàng ngoài giờ; `#3` Tóm tắt tài liệu học tập; `#5` Hướng dẫn thủ tục hành chính; `#7` Tra cứu hướng dẫn và quy định trong Lab | Tiếp nhận yêu cầu bằng ngôn ngữ tự nhiên, tìm kiếm, tổng hợp và trình bày thông tin phù hợp với ngữ cảnh |
| **B — Tìm kiếm và kiểm chứng thông tin** | `#6` Tìm nhà cung cấp thay thế; `#8` Kiểm chứng trích dẫn trong bài nghiên cứu; `#9` Truy xuất cấu hình và lịch sử thí nghiệm ML | Tìm thông tin từ nhiều nguồn, so sánh, kiểm tra tính chính xác và truy xuất nguồn gốc |
| **C — Vận hành lặp lại theo quy trình** | `#2` Ghi nhận chi tiêu cá nhân; `#4` Cấp tài khoản và phân quyền nhân viên mới | Thực hiện các bước lặp lại theo quy tắc, biểu mẫu và điều kiện đã xác định |


### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian xử lý thủ công và giảm sai sót trong các tác vụ tra cứu, kiểm chứng thông tin và vận hành lặp lại
├── Opportunity A (từ Cluster A - #1, #3, #5, #7): Thông tin hướng dẫn/quy định dài và phân tán ở nhiều nơi, khiến người cần thông tin mất nhiều thời gian tự dò tìm hoặc phải chờ hỏi lại người phụ trách
├── Opportunity B (từ Cluster B - #6, #8, #9): Phải đối chiếu chéo thủ công giữa nội dung/kết quả đang làm với nhiều nguồn dữ liệu gốc (paper PDF, file log thí nghiệm, hồ sơ nhà cung cấp) nên tốn thời gian và dễ nhầm lẫn nguồn
└── Opportunity C (từ Cluster C - #2, #4): Các thao tác nhập liệu và cấp quyền theo quy tắc cố định phải làm tay lặp đi lặp lại qua nhiều bước, gây tốn thời gian và dễ bỏ sót bước
     ✗ "Chatbot trả lời khách hàng ngoài giờ / Chatbot hỏi đáp Lab" ← solution, gạch bỏ khỏi tầng này
     ✗ "Tool tự động kiểm tra trích dẫn / Hệ thống quản lý thí nghiệm" ← solution, gạch bỏ khỏi tầng này
     ✗ "Script tự động cấp tài khoản và phân quyền" ← solution, gạch bỏ khỏi tầng này 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- "Cần một Chatbot trực fanpage ngoài giờ (#1) hoặc trợ lý ảo hỏi đáp quy định Lab (#7)": Đã gạch bỏ vì đây là giải pháp công nghệ; pain thật sự là người dùng không tra cứu nhanh được câu trả lời đúng ngữ cảnh từ tài liệu sẵn có.
- "Làm công cụ tự động kiểm tra trích dẫn (#8) / Dashboard quản lý thí nghiệm (#9)": Đã gạch bỏ vì đây là tính năng sản phẩm; pain thật sự là việc mất hàng chục phút đối chiếu thủ công số liệu/cấu hình với nguồn gốc để tránh sai lệch.
- "Tự động hóa quy trình cấp tài khoản (#4)": Đã gạch bỏ vì "tự động hóa" là cách giải quyết; pain thật sự là thao tác tay lặp lại trên nhiều hệ thống theo một biểu mẫu cố định.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **#3 — Tóm tắt tài liệu học tập (200 trang slide ôn thi)** | 5 | 5 | 5 | 4 | 5 | 5 | 5 | **34** |
| **#2 — Ghi nhận và phân loại chi tiêu cá nhân** | 5 | 5 | 4 | 4 | 5 | 3 | 5 | **31** |
| **#5 — Hướng dẫn thủ tục hành chính cho người dân** | 4 | 4 | 4 | 3 | 2 | 5 | 3 | **25** |
| **#6 — Tìm nhà cung cấp thay thế khi hết tồn kho** | 4 | 4 | 3 | 4 | 2 | 4 | 3 | **24** |

**Candidate được chọn:** **`#3` — Tóm tắt tài liệu học tập (Trích xuất công thức và kiến thức cốt lõi từ slide bài giảng khi ôn thi cuối kỳ)** *(hoặc `#2` nếu nhóm chốt chọn bài toán chi tiêu cá nhân).*

**Vì sao chọn:**
- **Actor và Domain sát sườn 100% thành viên:** Cả nhóm đều là sinh viên/học viên trực tiếp trải qua nỗi đau đọc hàng trăm trang slide trước kỳ thi; quy trình hiện tại rất rõ từng bước và có sẵn dữ liệu thật (các bộ slide môn học).
- **Thuận lợi kiểm chứng thực tế ngay ở CP4:** Dễ dàng phỏng vấn trực tiếp người thật (các bạn học viên ở nhóm khác trong lớp theo đúng luật *The Mom Test*) và thu thập survey nhanh ngay trong 30 phút của buổi Lab mà không phải giả định.
- **Phân tầng rõ rệt giữa No AI / Rule / Workflow / Agent:** Dễ dàng đặt lên bàn cân giữa giải pháp không dùng AI (dùng bản tóm tắt khóa trên, mục lục chuẩn), Rule (script gom text từ PDF/PPTX), và Workflow AI (trích xuất khái niệm/công thức theo chương + con người kiểm tra lại công thức toán/hình vẽ).

**Vì sao loại các candidate còn lại:**
- **Loại `#5` (Hướng dẫn thủ tục hành chính):** Dù pain point xã hội rất lớn và rất hay để so sánh giữa Decision Tree (Rule) với AI, nhưng trong khuôn khổ 4 tiếng của buổi Lab, nhóm không thể tiếp cận phỏng vấn trực tiếp "cán bộ tiếp nhận hồ sơ" thật ở CP4. Ngoài ra, bài toán có rủi ro pháp lý cao (Viability) khi văn bản pháp luật thay đổi liên tục.
- **Loại `#6` (Tìm nhà cung cấp thay thế khi hết hàng):** Quy trình phụ thuộc nhiều vào yếu tố bên ngoài (các nhà cung cấp truyền thống không mở API tồn kho thời gian thực mà phải gọi điện/nhắn Zalo hỏi tay). Nhóm cũng khó tìm được nhân viên thu mua (Procurement) thực tế để phỏng vấn kiểm chứng ngay trong giờ Lab.
- **Loại `#2` (Ghi nhận chi tiêu cá nhân):** Đạt điểm rất cao (32/35) và dễ kiểm chứng, nhưng trên thị trường đã có quá nhiều ứng dụng giải quyết tốt bằng Rule/tích hợp biến động số dư ngân hàng (Money Lover, MISA, app ngân hàng). Phần bottleneck thực sự còn lại chủ yếu nằm ở thói quen/động lực duy trì của người dùng hơn là bài toán kỹ thuật cần tới AI.

**Xử lý bất đồng (nếu có):**
- Một số thành viên ấn tượng với tính thực tiễn doanh nghiệp/xã hội của **`#5` (Thủ tục hành chính)** và **`#6` (Nhà cung cấp thay thế)**, trong khi thành viên khác nghiêng về **`#2` (Chi tiêu cá nhân)** và **`#3` (Tóm tắt tài liệu học tập)** vì có thể phỏng vấn người thật ngay tại lớp ở CP4. Nhóm đã thống nhất chấm điểm khách quan trên 7 tiêu chí, ưu tiên tiêu chí *"Vừa sức lab"* và *"Có thể kiểm chứng bằng hành vi người thật ngay tại lớp (CP4)"* để chốt chọn **`#3`** (và giữ `#2` làm phương án dự phòng sát nhất).

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Sinh viên ôn thi cuối kỳ thực sự mất 3–5 tiếng để lật giở đọc lại toàn bộ slide (>150–200 trang) để lọc công thức/kiến thức, và họ thực sự cần một bản tóm tắt trích xuất mới thay vì dùng lại tài liệu tóm tắt có sẵn từ khóa trước (No AI). | Value | 5 | 2 | ✅ |
| 2 | Bottleneck gây tốn thời gian nhất là bước đọc lướt, định vị và gõ lại công thức/định nghĩa cốt lõi sang file tổng hợp (chứ không phải bước học thuộc lòng hay làm bài tập). | Value | 4 | 2 | ✅ |
| 3 | AI (Multimodal LLM / OCR) có thể đọc và trích xuất chính xác công thức toán, ký hiệu chuyên ngành và sơ đồ từ slide dạng PDF/PPTX mà không bị ảo giác (hallucination) hay viết sai công thức. | Feasibility | 5 | 2 | ✅ |
| 4 | Sinh viên sẵn sàng tin tưởng và sử dụng bản tóm tắt do hệ thống tạo ra để ôn thi (nếu có trích dẫn số trang slide gốc đối chiếu) mà không cần phải tự lật giở đọc lại toàn bộ từng trang slide từ đầu. | Usability | 5 | 1 | ✅ |
| 5 | Chi phí xử lý token/API trên mỗi bộ slide (150–200 trang) đủ rẻ (< 5.000 – 10.000 VNĐ/bộ môn) hoặc có thể tận dụng các mô hình/công cụ miễn phí để sinh viên sẵn sàng sử dụng. | Viability | 4 | 3 | — |
| 6 | Slide bài giảng của trường/giảng viên không bị ràng buộc nghiêm ngặt về bản quyền hoặc bí mật đề thi, cho phép sinh viên đưa vào các công cụ AI để xử lý học tập cá nhân. | Viability | 3 | 3 | — |

Giả định nhóm kiểm chứng trong buổi này:
- **Giả định #1 (Value) & Giả định #4 (Usability):** Đây là hai giả định có **Độ quan trọng cao (5/5)** nhưng **Bằng chứng còn thấp (1–2/5)**. Nếu sinh viên có thói quen chỉ xin tài liệu khóa trên hoặc không tin tưởng bản tóm tắt tự động (vẫn phải đọc lại từ đầu vì sợ trượt môn), bài toán sẽ hoàn toàn sụp đổ. Nhóm sẽ kiểm chứng bằng phỏng vấn trực tiếp sinh viên/học viên trong lớp theo phương pháp *The Mom Test* ngay tại CP4.
- **Giả định #3 (Feasibility):** Kiểm chứng nhanh bằng cách lấy mẫu thử 5–10 trang slide có chứa công thức toán phức tạp và sơ đồ từ tài liệu thật của các thành viên để kiểm tra khả năng trích xuất của mô hình.

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

[Interview snapshot](../assets/cp4-interview-snapshot.md):

| Nguồn                                                             | Số người / số mẫu | Tín hiệu xác nhận                                                                                                                                                   | Tín hiệu phản bác                                                                                                                                                                      |
| ----------------------------------------------------------------- | ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Phỏng vấn 1 – Sinh viên gặp khó khăn về thuật ngữ song ngữ        | 1                 | Giáo trình tiếng Anh và slide tiếng Việt sử dụng cách diễn giải khác nhau; sinh viên khó thống nhất thuật ngữ và tổng hợp kiến thức để ôn thi.                      | Chưa chứng minh nhu cầu tóm tắt tự động; vấn đề cốt lõi có thể là chuẩn hóa thuật ngữ và cách diễn giải.                                                                               |
| Phỏng vấn 2 – Sinh viên không nhận biết được lỗ hổng kiến thức    | 1                 | Đọc bản tóm tắt tạo cảm giác hiểu bài nhưng không thể vận dụng khi thi; sinh viên không biết mình còn yếu ở đâu.                                                    | Tóm tắt tài liệu đơn thuần không giải quyết được vấn đề; nhu cầu thực tế nghiêng về kiểm tra mức độ hiểu và phát hiện lỗ hổng kiến thức.                                               |
| Phỏng vấn 3 – Sinh viên khó vận dụng công thức vào bài tập        | 1                 | Tóm tắt chỉ liệt kê công thức chưa đủ để giải bài; sinh viên cần dạng bài mẫu và hướng dẫn cách lựa chọn, áp dụng công thức.                                        | Nhu cầu có thể nằm ở luyện tập theo dạng bài và hướng dẫn giải, không phải tổng hợp tài liệu.                                                                                          |
| Phỏng vấn 4 – Sinh viên cần tổng hợp công thức toán học chính xác | 1                 | Mất 4,5–5 giờ tổng hợp công thức cho một môn; phải chụp và nhập lại công thức thủ công. Có nhu cầu rõ về độ chính xác ký hiệu và khả năng đối chiếu số trang nguồn. | Không dám tin bản tóm tắt trên mạng vì sợ sai dấu trừ, chỉ số dưới. Nếu không bảo đảm độ chính xác, người học vẫn chọn làm thủ công.                                                   |
| Phỏng vấn 5 – Sinh viên chỉ cần tự tổng hợp khi tài liệu thay đổi | 1                 | Mất khoảng 3 giờ tự làm đề cương khi giảng viên đổi giáo trình hoặc slide mới.                                                                                      | Khi có đề cương tốt từ khóa trước, sinh viên ưu tiên dùng lại thay vì tự tổng hợp. Nhu cầu không xuất hiện ở mọi môn học; giải pháp phải tạo giá trị vượt trội so với tài liệu có sẵn. |

**Nhận định sau kiểm chứng**

Tín hiệu xác nhận:

- Sinh viên thực sự mất thời gian trong việc tổng hợp và hệ thống hóa tài liệu, đặc biệt với môn có nhiều công thức hoặc tài liệu mới.
- Việc tóm tắt đơn thuần chưa đáp ứng đầy đủ nhu cầu ôn thi.
- Độ chính xác, khả năng truy xuất về tài liệu gốc và khả năng hỗ trợ vận dụng kiến thức là những yêu cầu quan trọng.

Tín hiệu phản bác:

- Không phải sinh viên nào cũng cần tự tổng hợp tài liệu; đề cương từ khóa trước có thể giải quyết vấn đề với chi phí gần như bằng 0.
- Một số pain liên quan đến kiểm tra kiến thức, luyện tập dạng bài hoặc chuẩn hóa thuật ngữ, không trực tiếp thuộc bài toán tóm tắt.
- Sinh viên không sẵn sàng tin tưởng kết quả tự động nếu không thể kiểm chứng độ chính xác.

**Nhóm đã sửa problem thế nào sau kiểm chứng?**

Nhóm thu hẹp problem từ “Sinh viên mất nhiều thời gian tóm tắt tài liệu học tập trước kỳ thi” thành:

> Sinh viên gặp khó khăn trong việc tự tổng hợp và hệ thống hóa kiến thức ôn thi từ các tài liệu dài, phân tán hoặc mới cập nhật, đặc biệt khi cần bảo đảm tính chính xác của công thức, thuật ngữ và khả năng đối chiếu với tài liệu gốc.

Đồng thời, nhóm xác định rõ phạm vi:

1. Đối tượng ưu tiên: Sinh viên có môn học sử dụng nhiều tài liệu, công thức hoặc giáo trình/slide mới mà chưa có đề cương đáng tin cậy từ khóa trước.
2. Pain trọng tâm: Tốn thời gian tự tổng hợp kiến thức và khó bảo đảm bản tổng hợp chính xác, đầy đủ.
3. Điều kiện để giải pháp có giá trị: Kết quả phải giữ đúng ký hiệu, thuật ngữ, có nguồn và số trang để đối chiếu.
4. Chưa gộp vào problem chính: Kiểm tra lỗ hổng kiến thức và luyện tập dạng bài. Đây là những opportunity liên quan nhưng cần kiểm chứng riêng, vì có thể đòi hỏi một bài toán khác với tổng hợp tài liệu.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Google NotebookLM** | [https://notebooklm.google/](https://notebooklm.google/) | Tải tập tài liệu nguồn (nhiều file slide/giáo trình PDF) để hỏi đáp, tổng hợp theo chương và tạo tài liệu ôn tập (*Study Guide, FAQ, Audio Overview*) | Miễn phí; gắn citation trực tiếp về đoạn/trang nguồn giúp người học kiểm tra lại thông tin; hỗ trợ đa dạng đầu ra học tập | Citation chỉ trỏ về nguồn chứ không bảo đảm mọi câu trả lời đều diễn giải đúng 100%; vẫn cần con người kiểm tra lại công thức toán, các bước biến đổi và nội dung nằm trong hình ảnh/sơ đồ | Tận dụng cơ chế gắn citation theo trang nguồn làm tiêu chuẩn bắt buộc (Boundary), nhưng phải bổ sung bước kiểm chứng công thức và hình vẽ thay vì tin tuyệt đối vào bản tóm tắt tự động |
| **Claude (Projects)** | [https://claude.ai/](https://claude.ai/) | Duy trì ngữ cảnh học tập xuyên suốt nhiều tài liệu liên quan trong một Project; giải thích khái niệm khó, diễn giải công thức và tổng hợp kiến thức theo khung đề cương | Khả năng diễn giải logic, chuẩn hóa thuật ngữ song ngữ (Anh – Việt) và trình bày lại cấu trúc kiến thức rất rõ ràng | Khả năng xử lý phụ thuộc lớn vào loại file: đọc tốt PDF có lớp văn bản (text-based), nhưng với PDF chứa nhiều hình ảnh, sơ đồ phức tạp hoặc bản scan thì dễ bỏ sót chi tiết hoặc nhận diện lệch ký hiệu nếu không kiểm tra kỹ | Không được mặc định mọi loại PDF slide đều được AI xử lý như nhau; cần phân loại rõ bước xử lý văn bản và bước xử lý công thức/hình ảnh trong quy trình |
| **Mathpix Snip** | [https://mathpix.com/](https://mathpix.com/) | Nhận diện (OCR) công thức toán học, bảng biểu từ ảnh chụp/slide PDF và chuyển đổi tài liệu khoa học sang định dạng có cấu trúc (LaTeX, Markdown, DOCX) | Độ chính xác cực cao với ký hiệu toán học, chỉ số dưới, ma trận và biểu thức phức tạp (giải quyết trực tiếp nỗi sợ sai dấu/ký hiệu của Phỏng vấn #4) | Là công cụ chuyển đổi định dạng chuyên biệt, không thay thế được việc hiểu ngữ cảnh kiến thức, liên kết giữa các chương hay xây dựng lộ trình ôn tập | Với các môn nặng công thức toán, nên dùng công cụ OCR chuyên biệt như Mathpix ở bước trích xuất ký hiệu thay vì bắt LLM thông thường tự đọc ảnh công thức |
| **Adobe Acrobat AI Assistant** | [https://www.adobe.com/acrobat/generative-ai-pdf.html](https://www.adobe.com/acrobat/generative-ai-pdf.html) | Đọc, hỏi đáp và tóm tắt trên nhiều file PDF bài giảng cùng lúc thông qua *PDF Spaces* (ví dụ: gom 5 file PDF Đại số tuyến tính để tổng hợp toàn bộ phần *Eigenvalues* theo từng chương) | Trả lời kèm citation bấm vào là nhảy thẳng đến đúng vị trí nội dung trên trang PDF gốc; giao diện tối ưu cho người đọc trực tiếp trên slide/PDF | Không chuyên sâu về mặt sư phạm (như phân loại dạng bài tập hay thiết kế lộ trình ôn thi); tính năng AI nâng cao yêu cầu gói trả phí hàng tháng | Trải nghiệm "bấm vào trích dẫn nhảy ngay tới trang slide gốc" là mẫu UX chuẩn để sinh viên đối chiếu nhanh công thức mà không mất công lật tìm thủ công |
| **SciSpace** | [https://scispace.com/](https://scispace.com/) | Đọc tài liệu khoa học/giáo trình học thuật, giải thích thuật ngữ chuyên ngành và phần *Mathematical Formulation* ngay trên vùng văn bản/công thức được bôi đen | Câu trả lời gắn chặt với đoạn nguồn được chọn; hỗ trợ đa ngôn ngữ (giải quyết tốt pain point đối chiếu thuật ngữ Anh – Việt ở Phỏng vấn #1) | Tập trung sâu vào phân tích từng bài báo/tài liệu học thuật đơn lẻ hơn là tổ chức và hệ thống hóa toàn bộ giáo trình/slide cả học kỳ thành một đề cương ôn thi thống nhất | Học hỏi cơ chế giải thích thuật ngữ song ngữ và giải nghĩa từng biến số trong công thức ngay tại chỗ để tích hợp vào quy trình tổng hợp đề cương |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

```text
HIỆN TẠI — Khi chưa có đề cương khóa trước đáng tin cậy; khoảng 3–5 giờ/môn

[1. Kiểm tra tài liệu ôn tập có sẵn; nếu không đủ tin cậy, lấy slide/giáo trình mới: 5']
  → [2. Lướt tài liệu dài để nhận biết chương và định vị nội dung cần ôn: 15']
  → [3. Đọc dò, chọn kiến thức cốt lõi rồi tự gõ/chụp công thức, định nghĩa sang đề cương: ~210'] ← BOTTLENECK
  → [4. Mở lại tài liệu gốc để kiểm tra ký hiệu, biến số, ngữ cảnh và phần bị bỏ sót: ~30']
  → [5. Hoàn thiện đề cương để dùng khi ôn thi: ~10']

Trường hợp có đề cương khóa trước đáng tin cậy, sinh viên có thể dùng lại và không thực hiện toàn bộ quy trình này.
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Sinh viên | Slide/giáo trình hiện tại và đề cương hoặc tài liệu từ khóa trước (nếu có) | Quyết định dùng tài liệu sẵn có hay tự tổng hợp từ bộ tài liệu mới | Khoảng 5 phút / môn | Nếu đề cương cũ đáng tin cậy thì có thể bỏ qua phần lớn công việc tự tổng hợp; pain tập trung ở môn có tài liệu mới hoặc chưa có bản tổng hợp phù hợp. |
| 2 | Sinh viên | Bộ slide/giáo trình dài, thường trên 200 trang theo candidate được chọn | Nhận biết cấu trúc chương và các phần cần ôn | Khoảng 15 phút / môn | Lướt tài liệu để định vị nội dung; tài liệu có thể dài hoặc chưa có cấu trúc ôn tập phù hợp. |
| 3 | Sinh viên | Slide/giáo trình theo chương | Đề cương cá nhân gồm kiến thức cốt lõi, định nghĩa và công thức | Khoảng 210 phút / môn; tổng thời gian được ước tính khoảng 3–5 giờ tùy môn | **Bottleneck chính:** phải đọc dò, chọn lọc rồi gõ lại hoặc chụp công thức/định nghĩa thủ công. Đây là phần mất thời gian nhất; công thức và thuật ngữ chuyên ngành cũng dễ bị ghi thiếu hoặc sai. |
| 4 | Sinh viên | Đề cương đang làm và slide/giáo trình gốc | Nội dung đã đối chiếu được ký hiệu, biến số, ngữ cảnh và nguồn | Khoảng 30 phút / môn | Khi thiếu ngữ cảnh hoặc lo ngại sai ký hiệu, sinh viên phải tìm lại trang gốc. Cần truy xuất được nguồn để kiểm tra độ chính xác, nhất là với công thức và hình/sơ đồ. |
| 5 | Sinh viên | Đề cương đã tổng hợp và đối chiếu | Tài liệu dùng để ôn thi | Khoảng 10 phút / môn | Hoàn thiện định dạng để đọc, in hoặc mở trên thiết bị; đây không phải pain trọng tâm. |

**Bottleneck chính:** Bước 3 ước tính chiếm khoảng 78% thời gian soạn tài liệu, kéo theo bước 4 phát sinh thêm thời gian để kiểm tra độ chính xác và tìm lại nguồn. Điều này khớp với kết quả CP4: nhu cầu không chỉ là tóm tắt nhanh, mà còn phải đáng tin cậy và đối chiếu được với tài liệu gốc.

### 4.2. Quy trình tương lai


```text
TƯƠNG LAI — Workflow hỗ trợ tổng hợp; chỉ áp dụng khi chưa có đề cương khóa trước đáng tin cậy

[1. Con người: Chọn slide/giáo trình cần ôn và xác nhận được phép dùng công cụ xử lý: ~5']
  → [2. Rule: Trích xuất văn bản/OCR, chia theo chương và giữ thông tin trang nguồn;
     con người kiểm tra nhanh file scan hoặc trang trích xuất lỗi: ~15']
  → [3. AI: Tạo bản nháp đề cương theo chương, nêu khái niệm/công thức cốt lõi
     và gắn trang nguồn để tra cứu; không tự thêm kiến thức ngoài tài liệu: ~20–30'] ← GIẢM BOTTLENECK
  → [4. Con người: Đối chiếu công thức, ký hiệu, thuật ngữ, độ bao phủ và trích dẫn
     với slide gốc; sửa hoặc bổ sung phần sai/thiếu: ~40–50']
  → [5. Con người: Hoàn thiện đề cương để ôn thi: ~10']

Boundary: Không dùng bản nháp AI như đáp án đã xác thực; mọi công thức, nội dung trích từ
hình/sơ đồ và phần không có trích dẫn rõ ràng phải được kiểm tra trên slide gốc.
Nếu trích xuất hoặc AI sai/thiếu, bỏ phần lỗi và tự đọc, chép lại từ tài liệu gốc như quy trình hiện tại.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 5 | Cùng phạm vi: một môn chưa có đề cương khóa trước đáng tin cậy. |
| Tổng thời gian | ~270 phút (ước tính; khoảng 3–5 giờ tùy môn) | ~90–110 phút mục tiêu | Ước tính ban đầu, cần đo thử trên bộ slide thật |
| Số bước thủ công | 5/5 | 3/5 hoàn toàn thủ công; bước 2 có kiểm tra thủ công | Bước 3 chuyển việc tạo bản nháp sang AI; người học vẫn kiểm tra và chịu trách nhiệm nội dung cuối. |
| Bottleneck chính | Đọc dò và tự gõ/chụp kiến thức cốt lõi (~210 phút) | Đối chiếu độ chính xác, nhất là công thức và nội dung từ hình (~40–50 phút) | Không cắt giảm bước kiểm tra để đổi lấy tốc độ; trích dẫn trang giúp tìm lại nguồn nhanh hơn. |
| Rủi ro mới phát sinh | Sai sót khi chép tay, bỏ sót kiến thức | AI/OCR có thể viết sai ký hiệu, bỏ sót nội dung hoặc gắn nguồn không khớp | Kiểm tra với slide gốc; nếu không xác minh được thì tự xử lý phần đó theo quy trình hiện tại. |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên ôn thi một môn có slide/giáo trình dài hoặc mới cập nhật và chưa có đề cương khóa trước đáng tin cậy. |
| **Quy trình** | Sinh viên kiểm tra tài liệu có sẵn, chọn slide/giáo trình cần ôn, rồi tự đọc, chọn lọc và gõ/chụp kiến thức thành đề cương; sau đó tra lại tài liệu gốc để kiểm tra công thức, thuật ngữ và phần bị bỏ sót. Công cụ được đề xuất hỗ trợ trích xuất/chia tài liệu và tạo bản nháp có dẫn trang; sinh viên rà soát, chỉnh sửa và hoàn thiện bản dùng để ôn. |
| **Bottleneck** | Tự đọc dò và tổng hợp thủ công kiến thức cốt lõi, đặc biệt là công thức và thuật ngữ; bước này được ước tính khoảng 210 phút/môn. Việc tìm lại trang gốc để xác minh nội dung cũng phát sinh thêm thời gian. |
| **Impact** | Quy trình hiện tại mất khoảng 3–5 giờ/môn theo ước tính của nhóm, làm giảm thời gian dành cho ôn tập và khiến sinh viên dễ bỏ sót hoặc ghi sai kiến thức. Mục tiêu là giảm thời gian tạo đề cương nhưng vẫn giữ khả năng kiểm tra nội dung với tài liệu gốc. |
| **Success Metric** (baseline → target, cách đo) | Baseline ước tính ~270 phút; mục tiêu ban đầu 90–110 phút/môn. Đo thời gian thực tế từ lúc chọn tài liệu đến khi hoàn thiện đề cương đã rà soát trên cùng một bộ slide/giáo trình. Đồng thời, lập trước checklist các ý chính và mẫu công thức cần có, rồi đối chiếu đề cương với tài liệu gốc: ghi nhận nội dung bị bỏ sót, công thức/ký hiệu sai và trích dẫn không truy được về nguồn. Tiêu chí chất lượng tối thiểu của mẫu là không có lỗi trọng yếu về công thức/ký hiệu và mọi nội dung được lấy mẫu đều truy được về nguồn; theo dõi độ bao phủ bằng checklist. Mục tiêu thời gian và chất lượng đều cần thử nghiệm, chưa phải kết quả đã xác nhận. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI chỉ tạo bản nháp dựa trên tài liệu đầu vào, không tự thêm kiến thức ngoài nguồn hoặc được xem là đáp án đã xác thực. Sinh viên phải kiểm tra công thức, ký hiệu, nội dung từ hình/sơ đồ, độ bao phủ và trích dẫn với tài liệu gốc; phần sai, thiếu nguồn hoặc không xác minh được phải tự xử lý theo quy trình hiện tại. Bản tạo ra mặc định thuộc về cá nhân; chỉ chia sẻ tự nguyện sau khi rà soát, ghi rõ môn/học kỳ/phiên bản tài liệu và được phép chia sẻ. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

1. Sẽ có nhiều người cùng ôn một môn. Có nên tính đến việc xây dựng một kho chung để chỉ cần một người làm đề cương, những người khác có thể dùng theo đề cương chuẩn đó không?
- **Phản biện của nhóm:** Ý tưởng kho chung nằm ngoài phạm vi hiện tại. Problem Statement v0 chỉ tập trung rút gọn quy trình mỗi sinh viên xây dựng đề cương từ tài liệu của mình; chưa giải quyết việc tạo, quản lý hay chọn một đề cương chuẩn dùng chung.
- **Hướng nối tiếp:** Có thể phát triển một hệ thống chia sẻ, nơi nhiều phiên bản đề cương được đăng song song và cộng đồng sinh viên đánh giá để giúp người học lựa chọn bản phù hợp cho việc ôn thi. Đây là hướng phát triển sau, không phải phần của giải pháp đang xác định.
2. Nếu chỉ đo thời gian tạo đề cương thì chưa biết bản nháp có đủ chính xác và đầy đủ để dùng ôn tập hay không; cần có tiêu chí chất lượng, không chỉ tiêu chí tốc độ.
- **Nhóm đồng ý:** Bổ sung đánh giá chất lượng bằng cách đối chiếu một checklist ý chính và mẫu công thức với tài liệu gốc, ghi nhận nội dung bỏ sót, lỗi công thức/ký hiệu và trích dẫn không truy được nguồn. Thời gian mục tiêu chỉ có ý nghĩa khi mẫu kiểm tra không có lỗi trọng yếu về công thức/ký hiệu và các nội dung được lấy mẫu đều truy được về nguồn; độ bao phủ được theo dõi bằng checklist.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ Trung bình–Cao × Độ phức tạp Trung bình**

Vì sao:
- **Độ mơ hồ Trung bình–Cao:** Việc rút gọn một chương slide 30–50 trang thành đề cương cô đọng, giải nghĩa biến số và thống nhất thuật ngữ song ngữ (Anh – Việt) giữa giáo trình với slide không có một bộ quy tắc `if-else` cố định (nhiều cách diễn đạt và cấu trúc tóm tắt khác nhau đều chấp nhận được). Tuy nhiên, riêng phần **ký hiệu toán học, công thức và số trang trích dẫn** lại đòi hỏi tính chính xác tuyệt đối (đúng/sai rõ ràng).
- **Độ phức tạp Trung bình:** Quy trình thực hiện gồm 5 bước nối tiếp cố định (Chọn tài liệu $\rightarrow$ Trích xuất văn bản/OCR theo chương $\rightarrow$ Tạo bản nháp đề cương có gắn trang nguồn $\rightarrow$ Con người đối chiếu và sửa $\rightarrow$ Hoàn thiện). Luồng đi hoàn toàn xác định trước, xử lý trên một tập tài liệu đóng (slide/giáo trình của môn học), không cần hệ thống tự động lập kế hoạch đa nhánh hay tự ý gọi các hệ thống bên ngoài.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Xin và dùng lại đề cương từ khóa trước; hoặc nhóm bạn học chia nhau mỗi người tự tóm tắt 1–2 chương theo cùng một khung mẫu (template) rồi ghép lại. | Khi môn học không đổi giáo trình/slide và đã có đề cương khóa trước đáng tin cậy (đúng như phát hiện ở Phỏng vấn #5). | Không giải quyết được khi giảng viên đổi slide/giáo trình mới, môn học ít người chia sẻ hoặc khi sinh viên vẫn phải tự đọc dò và gõ lại hàng chục công thức toán. | **Dùng ở Bước 1** (luôn kiểm tra xem có đề cương cũ tin cậy không trước khi làm mới) |
| **Rule** | Dùng công cụ trích xuất văn bản/OCR chuyên biệt (như *Mathpix Snip*, công cụ tách chương PDF, lọc trang có công thức) để gom text và chuyển ảnh công thức sang LaTeX/Markdown kèm số trang nguồn. | Khi chỉ cần chuyển đổi định dạng tài liệu (từ ảnh/PDF sang văn bản có cấu trúc) và giữ vị trí trang nguồn. | Không tự chọn lọc được đâu là kiến thức cốt lõi cần ôn, không liên kết được ngữ cảnh giữa các trang slide và không tự đối chiếu được thuật ngữ song ngữ Anh – Việt. | **Dùng cho Bước 2** (trích xuất văn bản/OCR công thức và giữ thông tin trang nguồn) |
| **Workflow** | Quy trình 5 bước định sẵn kết hợp **Rule + AI + Con người**: (1) Sinh viên chọn tài liệu $\rightarrow$ (2) Rule/OCR trích xuất text & công thức theo chương $\rightarrow$ (3) AI (*NotebookLM / Claude Projects / Adobe PDF Spaces*) tạo bản nháp đề cương có gắn `[Trang nguồn]` $\rightarrow$ (4) Sinh viên đối chiếu công thức, ký hiệu, hình vẽ với slide gốc và chỉnh sửa $\rightarrow$ (5) Hoàn thiện. | Khi các bước tổng hợp đã cố định, AI đóng vai trò rút ngắn bước tạo bản nháp (từ 210' xuống 20–30') và người học kiểm soát chất lượng cuối cùng. | AI/OCR có thể nhận diện sai chỉ số dưới, dấu trừ (`-`), bỏ sót điều kiện áp dụng công thức hoặc gắn lệch trang nguồn nếu người học chủ quan không kiểm tra. | **Chọn (Mức can thiệp chính)** |
| **Agent** | Hệ thống AI tự động quét toàn bộ kho học liệu, tự quyết định phần nào quan trọng cho kỳ thi, tự tìm thêm tài liệu bên ngoài để bổ sung và xuất thẳng đề cương hoàn chỉnh mà không cần con người duyệt từng chương. | Khi bài toán có luồng hành động mở, cần tự chủ tìm kiếm nhiều nguồn ngoài và không biết trước các bước xử lý. | Dễ đưa kiến thức ngoài phạm vi thi của giảng viên, rủi ro ảo giác (hallucination) công thức toán học và lấy mất bước kiểm chứng của người học (đi ngược lại yêu cầu cốt lõi của Phỏng vấn #4). | **Không chọn** |

**Mức chọn:** **Workflow** (Kết hợp **No AI** ở bước sàng lọc đầu vào + **Rule/OCR** ở bước trích xuất tài liệu/công thức + **AI** ở bước tạo bản nháp đề cương theo chương có gắn trang nguồn + **Con người** kiểm chứng).

**Vì sao không chọn mức đơn giản hơn:**
- Kết quả phỏng vấn ở CP4 cho thấy: với các môn đã có đề cương khóa trước tốt, nhóm khuyến nghị dừng ngay ở **No AI** (dùng lại tài liệu cũ). Tuy nhiên, với các môn mới cập nhật slide, tài liệu song ngữ Anh – Việt hoặc nặng về công thức (Phỏng vấn #1, #4, #5), **No AI** và **Rule** thuần túy (chỉ tách file/OCR) không giải quyết được **Bottleneck 210 phút** đọc lọc ý chính, chuẩn hóa thuật ngữ và hệ thống hóa kiến thức theo chương.
- Ngược lại, nhóm cũng không chọn **Agent** và không tự xây dựng phần mềm mới từ đầu, vì kết quả Research (mục 3.3) chỉ ra các công cụ sẵn có (*Google NotebookLM, Claude Projects, Mathpix, Adobe PDF Spaces*) đã đáp ứng tốt các mắt xích trong một **Workflow bán thủ công**.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Bản nháp đề cương ôn tập theo từng chương, gồm: (1) Khái niệm và định nghĩa cốt lõi (đã đối chiếu thuật ngữ Anh – Việt), (2) Danh sách công thức toán học kèm giải nghĩa biến số và điều kiện áp dụng, (3) Trích dẫn chính xác `[Tên file, Số trang/slide]` cho từng mục. |
| **Judgment** — con người cân nhắc, quyết định gì? | Sinh viên phán đoán và quyết định: (1) Công thức/ký hiệu toán học AI trích xuất có khớp 100% với slide gốc không, (2) Phần kiến thức nào là trọng tâm giảng viên nhấn mạnh trên lớp nhưng AI bỏ sót, (3) Nội dung nào từ hình vẽ/sơ đồ bị diễn giải sai cần sửa hoặc chép tay lại. |
| **Action** — hành động cuối cùng là gì, ai làm? | **Sinh viên** trực tiếp chỉnh sửa, bổ sung phần thiếu/sai trên bản nháp và chốt bản đề cương cuối cùng để sử dụng cho việc ôn thi. |
| **Outcome** — đo kết quả bằng gì? | (1) Tổng thời gian hoàn thiện đề cương (mục tiêu từ ~270 phút xuống 90–110 phút/môn); (2) Không có lỗi trọng yếu về công thức/ký hiệu trên mẫu kiểm tra sau rà soát; (3) 100% mục trong mẫu truy xuất được về đúng trang nguồn và đạt độ bao phủ theo checklist chương. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Bộ file slide bài giảng (PDF/PPTX), giáo trình môn học, đề cương môn học (Syllabus/mục lục chương) và văn bản/LaTeX đã qua bước OCR (nếu slide là ảnh chụp). **Đều có sẵn** từ học liệu môn học của sinh viên. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Tỷ lệ và loại lỗi mà sinh viên phải tự sửa ở Bước 4 (số công thức bị lỗi ký hiệu, số mục thiếu điều kiện áp dụng, số ý chính bị sót so với checklist chương) để tinh chỉnh lại cách chia nhỏ file và câu lệnh (prompt) cho các chương tiếp theo. |

### 6.4. Hai câu hỏi của Google PAIR

- **Người dùng muốn được hỗ trợ (augment) hay giao hẳn việc (automate)? Bằng chứng:**
  - Người dùng muốn **được hỗ trợ (Augment)**, tuyệt đối không muốn giao phó hoàn toàn (Automate).
  - **Bằng chứng từ CP4:** Ở Phỏng vấn #4, sinh viên khẳng định *“Không dám tin bản tóm tắt trên mạng vì sợ sai dấu trừ, chỉ số dưới; nếu không bảo đảm độ chính xác thì thà tự làm thủ công”*. Ở Phỏng vấn #2, sinh viên cũng chỉ ra việc chỉ đọc một bản tóm tắt có sẵn tạo ra *“cảm giác hiểu bài giả tạo nhưng vào phòng thi không làm được bài”*. Do đó, sinh viên cần AI làm nhanh phần việc nặng nhọc (lọc nháp và gắn số trang nguồn), còn bản thân bắt buộc phải tham gia vào bước đối chiếu và rà soát công thức (vừa để đảm bảo chính xác, vừa là một lần học chủ động).
- **AI sai kiểu nào tệ hơn, báo nhầm hay bỏ sót? Vì sao, và thiết kế đã xử lý thế nào:**
  - **Báo nhầm (ghi sai ký hiệu công thức, sai dấu `+/-`, sai điều kiện áp dụng hoặc gán sai nghĩa thuật ngữ nhưng trình bày rất thuyết phục)** tệ hơn vì nếu sinh viên không phát hiện ra, họ sẽ học thuộc công thức sai và mất điểm trực tiếp trong bài thi. Tuy nhiên, **bỏ sót (thiếu các định lý/công thức cốt lõi của chương)** cũng gây rủi ro lệch tủ khi ôn thi.
  - **Cách thiết kế xử lý cả hai:**
    1. *Chống báo nhầm (sai công thức/ảo giác):* Áp dụng Boundary buộc AI chỉ trích xuất từ tài liệu đầu vào và phải gắn `[Trang nguồn]` ngay cạnh từng công thức/định nghĩa; kết hợp công cụ OCR chuyên biệt (*Mathpix*) cho trang nhiều biểu thức toán và dành hẳn **Bước 4 (40–50 phút)** để sinh viên đối chiếu trực tiếp công thức với slide gốc.
    2. *Chống bỏ sót (thiếu ý chính):* Ở Bước 1 & 2, lập trước **Checklist các mục lớn/chương từ Syllabus/mục lục slide** để kiểm tra độ bao phủ của bản nháp; phần nào AI trích xuất lỗi hoặc thiếu nguồn thì quay về đọc và chép trực tiếp từ slide gốc (Fallback).

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên đại học các ngành kỹ thuật, khoa học tự nhiên, toán - tin ôn thi cuối kỳ các môn học có bài giảng slide dài (>150 trang), nhiều công thức và chưa có sẵn đề cương chuẩn khóa trước |
| **Quy trình** | Tải slide PDF → Rule tách cấu trúc chương → AI trích xuất danh mục công thức LaTeX & khái niệm cốt lõi kèm `[Slide p.XX]` → Sinh viên đối chiếu ảnh slide gốc và duyệt → Rule xuất file Cheat-sheet |
| **Bottleneck** | Bước đọc dò từng trang slide để định vị và gõ lại/chụp ảnh công thức toán sang file tổng hợp (mất 180–240 phút/môn) |
| **Impact** | Tốn 4–5 tiếng/môn; gây kiệt sức trước ngày thi; dễ gõ sai lệch ký hiệu toán hoặc bỏ sót công thức quan trọng |
| **Success Metric** (baseline → target, cách đo) | (1) Tổng thời gian tạo đề cương từ **240–300 phút xuống dưới 45 phút/môn** (sinh viên tự bấm giờ);<br>(2) **Tỷ lệ công thức toán chính xác >= 95%** (sinh viên chỉ cần sửa dưới 5% số công thức trong bước duyệt);<br>(3) **100% công thức trích xuất có số trang slide gốc chính xác** để đối chiếu được ngay. |
| **Boundary** | - AI không tự ý suy diễn công thức nằm ngoài slide bài giảng.<br>- AI không tự ý thay đổi ký hiệu của giảng viên.<br>- Không tự động xuất bản nếu chưa qua bước con người duyệt (HITL). |
| **AI intervention point** | Chen vào giữa Bước 2 (sau khi Rule đã phân tách cấu trúc slide) và Bước 4 (trước khi sinh viên tiến hành duyệt nội dung). |
| **Mức chọn** | **Workflow** |
| **Rủi ro & người kiểm tra** | Rủi ro AI nhận diện sai ký hiệu toán hoặc bỏ sót công thức trọng tâm → **Sinh viên tự kiểm tra và duyệt** từng mục thông qua giao diện đối chiếu với ảnh chụp slide gốc trước khi xuất bản. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| **Actor** | Sinh viên đại học ôn thi cuối kỳ chung chung | Thu hẹp vào sinh viên ngành kỹ thuật/toán ôn môn có slide >150 trang chưa có đề cương chuẩn khóa trước | Kết quả kiểm chứng (CP4) cho thấy sinh viên các môn xã hội hoặc môn đã có đề cương cũ thì No AI đã đủ tốt. |
| **Success Metric** | Chỉ đo thời gian: giảm từ 270' xuống dưới 60' | Bổ sung thêm metric chất lượng: tỷ lệ công thức chính xác >= 95% và 100% trích dẫn đúng số trang | Phản biện nhận được chỉ ra nếu chỉ nhanh mà công thức sai thì sinh viên sẽ trượt môn. |
| **Boundary & Rủi ro** | Chỉ nêu AI không tự giải bài tập | Nêu cụ thể ranh giới ký hiệu toán học và cơ chế con người kiểm tra đối chiếu qua ảnh chụp slide gốc | Đảm bảo tính khả thi và an toàn học thuật, giải tỏa triệt để nỗi sợ sai công thức của người học. |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | **Tính chính xác của công thức (Math Accuracy)** | Công thức trích xuất dưới dạng LaTeX đúng 100% ký hiệu, chỉ số trên/dưới, dấu toán học so với slide gốc. | Xuất hiện ký hiệu sai lệch, mất dấu âm/dương, hoặc AI tự ý đổi tên biến số so với slide. |
| 2 | **Tính truy xuất nguồn gốc (Traceability)** | 100% các công thức và khái niệm trích xuất đều có gắn kèm thẻ số trang slide `[Slide p.XX]` dẫn đúng đến trang chứa nội dung đó. | Không có số trang, hoặc số trang trích dẫn bị lệch so với trang thực tế trong file PDF. |
| 3 | **Độ bao phủ kiến thức trọng tâm (Coverage)** | Bao quát >= 90% các công thức, định lý và định nghĩa cốt lõi được giảng viên đóng khung hoặc tổng kết ở cuối mỗi chương. | Bỏ sót các công thức nền tảng trong slide bài giảng. |
| 4 | **Tính cô đọng và phân loại (Structure & Conciseness)** | Nội dung trích xuất được gom nhóm rõ ràng theo từng chương/mục; độ dài bản tóm tắt chỉ chiếm từ 10–15% dung lượng slide gốc. | Trích xuất lan man toàn bộ lời dẫn, ví dụ phụ; không phân cấp được mục lục chương. |


---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Trung bình** | Phỏng vấn CP4 (5 người) xác nhận sinh viên mất 3–5 giờ/môn khi phải tự tổng hợp môn nhiều công thức hoặc đổi slide mới; tuy nhiên nhu cầu **không xuất hiện ở mọi môn** (nếu đã có đề cương khóa trước tốt thì sinh viên dùng lại ngay với chi phí bằng 0). Do đó giá trị chỉ cao khi nhắm đúng vào các môn mới cập nhật tài liệu hoặc nặng công thức chưa có đề cương tin cậy. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **Thấp – Trung bình** | Sinh viên đã quen thao tác với PDF và các công cụ như *NotebookLM / Claude*. Nhờ yêu cầu bắt buộc gắn số trang nguồn cho từng mục, sinh viên dễ dàng lật lại đúng trang slide gốc để kiểm tra và sửa lại ký hiệu công thức trong khoảng 40–50 phút. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Trung bình** | Các công cụ có sẵn (*Google NotebookLM, Claude Projects, Adobe PDF Spaces, SciSpace, Mathpix*) đã giải quyết tốt phần đọc PDF văn bản và gắn citation. Rủi ro kỹ thuật nằm ở các bộ slide chứa nhiều công thức viết trong ảnh chụp độ phân giải thấp hoặc sơ đồ phức tạp dễ bị OCR/AI đọc nhầm ký hiệu. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **Thấp – Trung bình** | Sinh viên tự vận hành quy trình cho mục đích ôn tập cá nhân trên các gói miễn phí/sinh viên sẵn có (*NotebookLM* miễn phí, *Mathpix/Claude* dùng trong hạn mức). Rủi ro bản quyền học liệu được kiểm soát bằng nguyên tắc: tài liệu chỉ xử lý trong không gian cá nhân khi được phép và không phát tán công khai khi chưa được phép. |

### 8.2. Kết luận

**Quyết định:** **Go (Phạm vi nhỏ — Triển khai Pilot quy trình Workflow bán thủ công bằng các công cụ có sẵn, KHÔNG tự xây dựng phần mềm/agent mới)**

**Lý do:**
- Không có rủi ro nào ở mức **Cao**. Các rủi ro **Trung bình** (Value chỉ tập trung ở môn chưa có đề cương cũ; Feasibility với công thức trong ảnh chụp) đều đã được kiểm soát bằng **Boundary chặt chẽ** (bắt buộc gắn trang nguồn + giữ bước sinh viên đối chiếu 40–50 phút) và có thể kiểm chứng ngay bằng một đợt chạy thử (pilot) với chi phí bằng 0 trên các công cụ sẵn có.
- Kết quả Research ở CP4 chứng minh các công cụ như *NotebookLM*, *Claude Projects* và *Mathpix* đã giải quyết được từng mảnh ghép; việc tự lập trình một hệ thống mới từ đầu là dư thừa và không kinh tế.

**Nếu Go — pilot nhỏ nhất:**
- **Quy mô:** Thử nghiệm ngay trong 1 tuần trên **1 môn học thật có nhiều công thức/thuật ngữ và chưa có đề cương khóa trước** (khoảng 150–200 trang slide, chia làm 5–6 chương), với **3 sinh viên** thực hiện.
- **Cách làm (không viết code xây app):**
  1. Lập trước **checklist các mục chính và 15–20 công thức mẫu** từ mục lục bộ slide.
  2. Chia bộ slide PDF theo chương; với trang có công thức dạng ảnh khó đọc thì quét nhanh qua *Mathpix Snip*, sau đó đưa vào *Google NotebookLM* (hoặc *Claude Project*) cùng prompt chuẩn yêu cầu tạo bản nháp đề cương theo chương kèm `[Số trang nguồn]`.
  3. Sinh viên bấm giờ toàn bộ quá trình (từ lúc chuẩn bị file đến khi đối chiếu xong với slide gốc và sửa lỗi) và chấm bản nháp theo **4 tiêu chí đánh giá** ở Mục 7.

**Nếu Not Yet — cần kiểm chứng gì trước:** *(Không áp dụng vì nhóm chọn Go phạm vi nhỏ; tuy nhiên trong quá trình pilot sẽ đồng thời xác nhận lại baseline thời gian và mục tiêu thời gian trên dữ liệu bấm giờ thật).*

**Nếu No-Go — nên làm gì thay AI:** *(Áp dụng ngay cho các môn đã có đề cương khóa trước đáng tin cậy: dùng phương án **No AI** — xin lại đề cương khóa trên và chỉ tự ghi chú bổ sung các phần giảng viên nhấn mạnh thêm trên lớp).*

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):
- **Về thời gian & công sức sửa lỗi:** Nếu sau khi thử nghiệm trên **2 chương đầu tiên (hoặc 1 môn học)** mà tổng thời gian (tạo nháp + đối chiếu sửa lỗi) **vẫn vượt quá 180 phút/môn**, hoặc sinh viên phải **viết/gõ lại thủ công trên 40% số công thức** do AI/OCR trích xuất lỗi $\rightarrow$ **Dừng dùng AI tạo nháp cho phần công thức**, quay về phương án cắt dán trực tiếp ảnh chụp công thức từ slide gốc vào đề cương và chỉ dùng công cụ để lập mục lục trang nguồn.
- **Về độ chính xác học thuật:** Nếu sau bước rà soát (Bước 4) mà kiểm tra chéo với checklist vẫn phát hiện **từ 1 lỗi trọng yếu trở lên về công thức/ký hiệu bị lọt qua** (sai dấu, sai biến số, thiếu điều kiện áp dụng làm giải sai bài tập) $\rightarrow$ **Dừng quy trình dùng AI tóm tắt môn đó**, quay về quy trình tự đọc và ghi chép trực tiếp từ slide gốc.

---

## 9. Hạn chế và hướng tiếp theo

- **Hạn chế của buổi Discovery hiện tại:**
  - Con số baseline (~270 phút/môn) và thời gian mục tiêu hiện đang dựa trên ước lượng hồi tưởng từ các buổi phỏng vấn ở CP4, chưa được bấm giờ trực tiếp (time-tracking) song song trên cùng một bộ slide chuẩn.
  - Quy trình hiện tại mới giải quyết bài toán **tổng hợp và hệ thống hóa tài liệu chính xác**, chưa giải quyết được 2 nhu cầu liền kề mà người học nêu ra ở Phỏng vấn #2 và #3 là **tự kiểm tra lỗ hổng kiến thức (active recall/quiz)** và **hướng dẫn áp dụng công thức vào từng dạng bài tập**.
- **Hướng tiếp theo:**
  - Thực hiện ngay đợt **Pilot nhỏ nhất** trên 1 môn học thật của thành viên trong nhóm ở học kỳ này để đo đạc chính xác thời gian thực tế và tỷ lệ lỗi công thức ở Bước 3 & Bước 4.
  - Ở vòng Discovery tiếp theo, kiểm chứng riêng bài toán *"Sinh viên không nhận biết được lỗ hổng kiến thức sau khi đọc đề cương"* (từ Phỏng vấn #2) và bài toán *"Kho đề cương chia sẻ có đánh giá chéo của cộng đồng sinh viên"* (từ Phản biện #1 ở CP5).

## 10. Tài liệu tham khảo

- Google NotebookLM — Công cụ hỏi đáp và tổng hợp tài liệu có gắn trích dẫn nguồn: [https://notebooklm.google/](https://notebooklm.google/)
- Anthropic Claude (Projects) — Không gian làm việc duy trì ngữ cảnh trên nhiều tài liệu: [https://claude.ai/](https://claude.ai/)
- Mathpix Snip — Công cụ OCR nhận diện công thức toán học và chuyển đổi PDF khoa học sang LaTeX/Markdown: [https://mathpix.com/](https://mathpix.com/)
- Adobe Acrobat AI Assistant (PDF Spaces) — Đọc, tóm tắt và trích dẫn nhảy tới vị trí nguồn trên nhiều file PDF: [https://www.adobe.com/acrobat/generative-ai-pdf.html](https://www.adobe.com/acrobat/generative-ai-pdf.html)
- SciSpace — Hỗ trợ đọc tài liệu khoa học, giải thích thuật ngữ và biểu thức toán học: [https://scispace.com/](https://scispace.com/)
- Tài liệu hướng dẫn Lab Day 02: [docs/01-worksheet.md](../../docs/01-worksheet.md), [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md), [docs/03-international-frameworks.md](../../docs/03-international-frameworks.md) (Double Diamond, Jobs-to-be-Done, Opportunity Solution Tree — Teresa Torres, The Mom Test — Rob Fitzpatrick, Lean UX — Jeff Gothelf, Google PAIR Guidebook, Building Effective Agents — Anthropic, Four Big Risks — Marty Cagan).
