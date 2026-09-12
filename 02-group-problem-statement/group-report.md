# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|-----|-----------|-------------|---------------------------------------------------------------|
| 1   |Mai Văn Trường|2A202602983|facilitator, workflow, research, writer|
| 2   |Hồ Ngọc Mai|2A202602509|facilitator, workflow, research, writer|
| 3   |Vũ Quốc Huy|2A202602929|facilitator, workflow, research, writer|
| 4   |Nguyễn Hoàng Cường|2A202602473|facilitator, workflow, research, writer|
| 5   |Nguyễn Hữu Thành|2A202602813|facilitator, workflow, research, writer|
| 6   |Đặng Quang Hưng|2A202602719|facilitator, workflow, research, writer|
**Candidate problem nhóm chọn (1 câu):**

Trả lời câu hỏi tài chính phức tạp mất nhiều thời gian vì phải truy xuất nhiều bảng/tài liệu, trích số liệu + evidence rồi mới tính.

---

## Phase 3 — Group Convergence: từ 9-12 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Đặng Quang Hưng | Tự động hóa chuẩn hóa báo cáo tiến độ học viên sau buổi học (Post-class Student Progress Report) | Teaching Assistant (TA), Học viên / Phụ huynh | Chuyển hóa các ghi chú thô, viết tắt trong giờ thành nhận xét sư phạm hoàn chỉnh, cá nhân hóa cho từng học viên tốn nhiều sức lực và dễ bị trễ deadline | Workflow rất rõ và thực tế, tiết kiệm thời gian thấy rõ (từ 60' xuống 15'); phù hợp dạng Workflow LLM bóc tách text thô sang template cố định; rủi ro AI dễ bịa thêm ngữ cảnh nếu note quá vắn tắt, cần cơ chế human review chặt chẽ. |
| 2 | Đặng Quang Hưng | Tự động hóa rà soát và giải thích lỗi ngữ pháp/từ vựng lặp lại trong bài viết IELTS | Teaching Assistant (TA), Học viên luyện thi IELTS | Dò tìm thủ công và gõ lại cùng một kiểu giải thích cho các lỗi câu từ cơ bản chiếm hơn 60% thời gian chấm, làm tồn đọng bài chấm và giảm thời gian nhận xét tư duy lập luận | Pain point rất thật và giá trị cao, AI giải quyết tốt tầng ngữ pháp/từ vựng bề mặt để giải phóng sức người cho phần lập luận; cần lưu ý AI có thể gợi ý cấu trúc không tự nhiên theo ngữ cảnh bài thi IELTS. |
| 3 | Đặng Quang Hưng | Hệ thống hỗ trợ giải đáp thắc mắc kiến thức ngoài giờ cho học viên tự học | Học viên (đặc biệt là người đi làm), Teaching Assistant (TA) | Độ trễ phản hồi kéo dài (4–8 tiếng) do lệch khung giờ sinh hoạt khiến học viên đứt mạch học tập; TA bị phân mảnh thời gian ngoài giờ để trả lời các câu hỏi lặp lại | Ý tưởng hay, mô hình RAG bot tra cứu slide/giáo trình rất hợp lý; tuy nhiên scope hơi rộng và độ phức tạp cao hơn (dạng Agent), khó kiểm soát tính chính xác tuyệt đối nếu tài liệu bài giảng không đủ chuẩn hóa. |
| 4 | Vũ Quốc Huy | Sinh viên mất khoảng 3.5 giờ/môn để tổng hợp ghi chú từ slide, sách và video trước kỳ thi | Sinh viên phải ôn nhiều môn, đặc biệt các môn có nhiều nguồn tài liệu | Tự gộp và viết lại thông tin từ nhiều định dạng thành một bản tổng hợp | Impact cao, workflow rõ, có thể thử Workflow có AI; cần kiểm tra AI có bỏ sót hoặc hiểu sai kiến thức không |
| 5 | Vũ Quốc Huy | Thành viên nhóm thường hỏi lại task và deadline dù thông tin đã có trong tài liệu chung | Thành viên nhóm, leader và mentor | Leader phải tra cứu rồi trả lời lại, mất khoảng 20–30 phút/tuần | Pain lặp lại, nhưng Rule gửi reminder có thể đã đủ; cần kiểm tra có thật sự cần AI không |
| 6 | Vũ Quốc Huy | Sinh viên mất khoảng 30–45 phút/tuần để viết báo cáo tiến độ từ commit, notes và tin nhắn nhóm | Sinh viên làm đồ án, leader và giảng viên hướng dẫn | Thu thập thông tin rời rạc rồi chuyển thành báo cáo có cấu trúc | Workflow phù hợp để thử AI tạo bản nháp; cần kiểm tra dữ liệu đầu vào có đầy đủ không |
| 7 | Mai Văn Trường | Sinh viên mất nhiều thời gian chuyển code, kết quả test và log kỹ thuật thành một báo cáo có cấu trúc hoàn chỉnh. | Sinh viên làm bài thực hành, bài lab hoặc đồ án. | Phải tự đọc nhiều nguồn đầu vào rồi chọn nội dung và viết mô tả theo đúng cấu trúc báo cáo. | Vấn đề rõ, thường xuyên gặp, impact đo được và phù hợp để thử nghiệm AI hỗ trợ tạo bản nháp báo cáo. |
| 8 | Mai Văn Trường | Sau các buổi Meet/Discord, thông tin về quyết định, nhiệm vụ và deadline dễ bị phân tán hoặc bị quên. | Sinh viên làm bài tập nhóm hoặc đồ án theo team. | Không có cách ghi lại quyết định, action item, người phụ trách và deadline một cách nhất quán. | Có pain thật trong làm việc nhóm, workflow rõ; AI có thể hỗ trợ tổng hợp nhưng phụ thuộc vào transcript hoặc ghi chú đầu vào. |
| 9 | Mai Văn Trường | Sinh viên lập trình mất nhiều thời gian đọc log và thử nhiều cách sửa trước khi xác định được nguyên nhân chính của lỗi. | Sinh viên lập trình khi học, làm lab hoặc đồ án. | Khó phân biệt lỗi gốc với warning và các lỗi phát sinh phía sau trong log dài. | Problem thực tế, xảy ra thường xuyên và dễ đo bằng thời gian debug; AI có tiềm năng hỗ trợ nhưng cần kiểm soát độ chính xác. |
| 10 | Nguyễn Hữu Thành | Inbox/comment lặp câu hỏi, hay bỏ sót → mất 1–2 tiếng/ngày reply thủ công | Mẹ bỉm làm content affiliate/review part-time | 70% câu hỏi trùng nhưng vẫn phải gõ tay từng reply |
| 11 | Nguyễn Hữu Thành | Mỗi tuần phải nghĩ idea từ đầu → mất 2–3 tiếng brainstorm | Mẹ bỉm + nhân viên văn phòng làm content thêm | Không có kho idea có cấu trúc, không biết idea nào đã dùng/fail | 
| 12 | Nguyễn Hữu Thành | Trả lời câu hỏi tài chính phức tạp mất nhiều thời gian vì phải truy xuất nhiều bảng/tài liệu, trích số liệu + evidence rồi mới tính | Nhân viên phân tích tài chính / kiểm toán | 1 câu hỏi → nhiều chỉ tiêu → nhiều bảng → nhiều lần truy xuất và kiểm chứng thủ công | 
| 13 | Nguyễn Hoàng Cường | Nhập dữ liệu hóa đơn giấy vào phần mềm kế toán | Kế toán viên tài vụ | Bước 3: Nhập tay thủ công từng trường thông tin (MST, tiền hàng, VAT) vào MISA. | Độ khả thi cao [Workflow]: Công nghệ OCR đã khá hoàn thiện. Impact lớn: giảm rủi ro sai sót làm lệch sổ sách thuế. Chốt: ưu tiên làm trước vì bài toán rõ ràng, dễ đo lường. |
| 14 | Nguyễn Hoàng Cường | Phân loại và gán thẻ ticket hỗ trợ kỹ thuật | Nhân sự trực tổng đài (Line 1) | Bước 3: Đọc hiểu mô tả lỗi và chọn danh mục/gán thẻ thủ công trên Jira. | Tần suất cao [Automation]: có thể giảm đáng kể công việc thủ công. Rủi ro thấp vì nếu AI gán sai thẻ vẫn có quy trình fallback xử lý. Chốt: đáng thử nghiệm và dễ đánh giá hiệu quả. |
| 15 | Nguyễn Hoàng Cường | Tổng hợp báo cáo doanh thu tuần | Trưởng nhóm Sale | Bước 4: Phân tích số liệu, vẽ biểu đồ xu hướng và tự viết nhận xét định tính. | Bài toán phức tạp [Agent]: AI cần phân tích nguyên nhân doanh số tăng/giảm để tạo nhận xét phù hợp. Cần chuẩn hóa dữ liệu trước khi xử lý. Chốt: nên thực hiện sau khi các file dữ liệu nguồn đã được chuẩn hóa. |

### 3.2. Gom trùng / cluster (gom 9-12 ý thành 3-4 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A — Tổng hợp và tạo báo cáo từ nhiều nguồn | #1, #4, #6, #7, #15 | Người dùng phải lấy dữ liệu/ghi chú từ nhiều nguồn rời rạc, chọn thông tin quan trọng rồi chuyển thành một báo cáo hoặc bản tổng hợp có cấu trúc. | Đây là cụm có workflow rất rõ và dễ đo thời gian trước/sau. AI phù hợp để tạo draft, nhưng cần human review để tránh bỏ sót hoặc suy diễn sai dữ liệu. |
| B — Tự động hóa tác vụ lặp lại và phản hồi thường xuyên | #2, #3, #5, #8, #10, #14 | Người dùng phải đọc thông tin đầu vào rồi thực hiện một hành động lặp lại như trả lời câu hỏi, phân loại, gán task/tag hoặc nhắc lại thông tin đã có. | Tần suất cao, impact tích lũy lớn. Một số bài có thể chỉ cần Rule/Automation, nên cần kiểm tra xem AI thực sự cần thiết ở bước nào. |
| C — Trích xuất, tra cứu và phân tích thông tin để ra quyết định | #9, #12, #13 | Người dùng phải xử lý lượng thông tin lớn hoặc nhiều nguồn để tìm dữ liệu quan trọng, xác định nguyên nhân, trích xuất trường dữ liệu hoặc đưa ra kết luận. | AI/OCR có thể giảm đáng kể thời gian xử lý, nhưng độ chính xác là yếu tố quan trọng. Cần có evidence, nguồn gốc dữ liệu hoặc bước xác nhận của con người. |
| D — Hỗ trợ tạo và quản lý nội dung/ý tưởng | #11 | Người dùng phải liên tục nghĩ nội dung mới nhưng thiếu kho ý tưởng có cấu trúc và khó theo dõi ý tưởng nào đã dùng hoặc không hiệu quả. | Có khả năng dùng AI cho ideation, nhưng problem hiện còn khá rộng và impact khó đo hơn các cluster khác. Nên làm rõ workflow và dữ liệu đầu vào trước khi ưu tiên. |

### 3.3. Shortlist (giữ 2-3 bài trả lời được 7 câu hỏi worksheet)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| #7 — Tổng hợp báo cáo từ code, test và log | Actor và workflow rất rõ: sinh viên hoàn thành code/test → đọc log → chọn nội dung → viết báo cáo → review. Pain có thể đo bằng thời gian hiện tại khoảng 1–3 giờ/báo cáo và có thể so sánh trực tiếp với workflow có AI. Nhóm cũng quen domain vì đều có trải nghiệm làm bài lab/đồ án và viết báo cáo. | AI có thể mô tả sai kết quả test hoặc tự suy diễn nội dung không có trong log. Cần xác định template đầu vào và bắt buộc có bước human review trước khi sử dụng báo cáo. |
| #14 — Phân loại và gán thẻ ticket hỗ trợ kỹ thuật | Workflow ngắn và lặp lại với tần suất cao: nhận ticket → đọc mô tả → xác định loại lỗi → gán tag/team xử lý. Dễ tạo bộ dữ liệu mẫu và đo accuracy, thời gian xử lý trước/sau. Có thể so sánh rõ Rule-based với AI Classification/Workflow. | Nhóm chưa có nhiều dữ liệu ticket thực tế và hiểu biết domain CSKH có thể hạn chế. Cần xác định taxonomy/tag rõ ràng để đánh giá AI gán đúng hay sai. |
| #12 — Trả lời câu hỏi tài chính phức tạp từ nhiều bảng và tài liệu | Actor cụ thể là nhân viên phân tích tài chính/kiểm toán. Workflow có thể mô tả rõ: nhận câu hỏi → xác định chỉ tiêu cần tìm → tra nhiều bảng/tài liệu → trích số liệu và evidence → tính toán → kiểm chứng → trả lời. Bottleneck nằm ở việc phải truy xuất và đối chiếu nhiều nguồn thủ công, phù hợp để thử Retrieval + Workflow AI. | Rủi ro lớn nhất là AI lấy sai số liệu, dùng nhầm kỳ báo cáo hoặc tạo kết luận không có evidence. Cần bắt buộc trích nguồn, kiểm chứng phép tính và có human review trước khi sử dụng kết quả. |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #7 — Tổng hợp báo cáo từ code, test và log | 5 | 5 | 4 | 5 | 5 | 4 | 5 | 33 |
| #14 — Phân loại và gán thẻ ticket hỗ trợ kỹ thuật | 5 | 5 | 4 | 5 | 5 | 5 | 3 | 32 |
| #12 — Trả lời câu hỏi tài chính phức tạp từ nhiều bảng và tài liệu | 5 | 5 | 5 | 5 | 4 | 5 | 5 | 34 |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
#12 — Trả lời câu hỏi tài chính phức tạp từ nhiều bảng và tài liệu.

Người gặp vấn đề: Nhân viên phân tích tài chính / kiểm toán.

Điểm nghẽn chính: Khi nhận một câu hỏi tài chính, người dùng phải xác định nhiều chỉ tiêu liên quan, tra cứu qua nhiều bảng và tài liệu, trích đúng số liệu và evidence, thực hiện tính toán rồi kiểm chứng thủ công trước khi đưa ra câu trả lời.

```

**Vì sao chọn (4-5 câu):**

```text
Nhóm chọn bài toán #12 vì đây là vấn đề có actor, workflow và điểm nghẽn khá rõ ràng trong công việc phân tích tài chính/kiểm toán. Khi trả lời một câu hỏi tài chính phức tạp, người dùng thường phải tra cứu nhiều bảng và tài liệu, đối chiếu số liệu, thực hiện tính toán và kiểm chứng evidence trước khi đưa ra kết luận. Quy trình này tốn thời gian, dễ xảy ra sai sót khi lấy nhầm số liệu hoặc nhầm kỳ báo cáo và có thể đo được impact thông qua thời gian xử lý, số lần truy xuất tài liệu và độ chính xác của kết quả. Bài toán cũng phù hợp để thử nghiệm AI theo hướng Retrieval + Workflow, trong đó AI hỗ trợ tìm dữ liệu, trích evidence và tổng hợp câu trả lời nhưng vẫn giữ bước human review. Ngoài ra, nhóm có thể so sánh rõ hiệu quả giữa cách làm thủ công, rule-based, workflow AI và agent để đánh giá mức độ phù hợp của từng phương án.
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
#7 — Tổng hợp báo cáo từ code, test và log: Bài toán này có workflow rõ và gần với trải nghiệm của nhóm, nhưng phạm vi sử dụng chủ yếu tập trung vào sinh viên làm lab/đồ án nên impact chưa rộng bằng candidate #12. Ngoài ra, một phần đáng kể của bài toán có thể được giải quyết bằng template và script thông thường mà chưa cần AI ở mức độ cao. 

#14 — Phân loại và gán thẻ ticket hỗ trợ kỹ thuật: Bài toán có tần suất cao và dễ đo accuracy, nhưng nhóm chưa có nhiều dữ liệu ticket thực tế cũng như hiểu biết sâu về taxonomy và quy trình CSKH. Nếu dữ liệu đầu vào không đủ tốt, kết quả đánh giá có thể thiếu tính thực tế và khó phản ánh đúng môi trường vận hành thật.
```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text
Rule/Workflow/Agent và có giá trị ứng dụng thực tế cao hơn nếu giải quyết tốt.
```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Interview | 3 | "Mỗi câu hỏi phức tạp em phải mở ít nhất 3–4 file Excel và 2–3 bản PDF để tìm đúng số liệu, nhiều khi mất 30–45 phút chỉ cho một câu." — NV phân tích TC 2 năm. "Sai sót hay xảy ra nhất là lấy nhầm số liệu kỳ trước hoặc nhầm đơn vị, phải kiểm tra 2–3 lần mới yên tâm." — NV kiểm toán nội bộ. "Em sợ nhất là câu hỏi so sánh nhiều kỳ, phải mở từng file copy số liệu ra bảng riêng mới đối chiếu được." — NV phân tích TC 3 năm. | 1/3 người nói nếu công ty đã có dashboard BI chuẩn thì câu hỏi đơn giản đã được trả lời sẵn, chỉ câu ad-hoc mới tốn thời gian. | Nhóm bổ sung điều kiện: problem tập trung vào câu hỏi ad-hoc/phức tạp cần truy xuất đa nguồn, không phải câu đã có sẵn trên dashboard. |
| Survey / poll | 6 | 5/6 người xác nhận mất trên 25 phút/câu hỏi phức tạp. 4/6 đồng ý bước tốn thời gian nhất là "tìm và đối chiếu số liệu từ nhiều bảng/tài liệu". 5/6 cho rằng sẽ dùng tool AI nếu tool trích nguồn rõ ràng. | 2/6 người lo AI lấy sai số liệu hoặc nhầm kỳ báo cáo, gây hậu quả nghiêm trọng nếu không kiểm tra kỹ. | Nhóm bổ sung yêu cầu bắt buộc: AI phải trích dẫn nguồn (tên bảng, dòng, cột, kỳ) cho mọi số liệu đưa ra. |
| Log / ticket / review (nếu có) | 15 câu hỏi | Nhóm thu thập log từ 2 NV: 15 câu hỏi ad-hoc trong 2 tuần, thời gian trung bình 35 phút/câu, trung bình truy xuất 3.2 tài liệu/câu hỏi. | — | — |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text
Pain thật nằm ở bước truy xuất và đối chiếu nhiều nguồn tài liệu để tìm đúng số liệu: NV phải mở nhiều file, xác định đúng kỳ/chỉ tiêu, copy số liệu ra rồi tính toán và kiểm chứng thủ công. Sai sót phổ biến ở bước lấy nhầm kỳ hoặc nhầm đơn vị, không phải ở bước tính toán.
```

Bằng chứng đính kèm (nếu có): `02-group-problem-statement-survey.png`, `...-interview-notes.md`

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Microsoft Copilot for Finance | https://www.microsoft.com/en-us/microsoft-365/copilot/copilot-for-finance | Truy xuất dữ liệu từ Excel và tổng hợp báo cáo tài chính, tích hợp trong Excel/Outlook. | Tích hợp sâu hệ sinh thái Microsoft, truy cập trực tiếp Excel/SharePoint, hỗ trợ variance analysis. | Yêu cầu license M365 E3/E5 + add-on. Chỉ hoạt động trong hệ sinh thái Microsoft, không xử lý PDF scan hay file ngoài. | AI tài chính cần tích hợp nguồn dữ liệu thực tế. Tập trung truy xuất đa nguồn + trích dẫn nguồn gốc. |
| ChatGPT + Advanced Data Analysis | https://chat.openai.com | Phân tích dữ liệu khi người dùng upload file, viết code Python xử lý bảng tính tự động. | Linh hoạt, upload CSV/Excel để phân tích, viết code tính toán + tạo biểu đồ. | Phải upload thủ công, không lưu context giữa phiên. Có thể hallucinate số liệu, không trích dẫn vị trí chính xác trong file gốc. | Cần pipeline tự động thu thập dữ liệu. Phải bắt buộc trích nguồn (tên bảng, sheet, dòng, cột) cho mỗi số liệu. |
| RAG pattern (LlamaIndex / LangChain) | https://docs.llamaindex.ai/en/stable/ | Tìm kiếm và trích xuất thông tin từ kho tài liệu lớn qua embedding + vector search trước khi sinh câu trả lời. | Tìm kiếm nhiều tài liệu cùng lúc, trích dẫn nguồn gốc, giảm hallucination bằng dữ liệu thực tế. | Chất lượng phụ thuộc cách chunk/index. Bảng số liệu tài chính khó embedding chính xác. Cần tiền xử lý cẩn thận. | RAG là pattern phù hợp nhất. Cần đầu tư tiền xử lý tài liệu tài chính và thiết kế retrieval phù hợp cấu trúc bảng số liệu. |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text
Các tool hiện có đều giải quyết được một phần nhưng thiếu khả năng truy xuất đa nguồn tài liệu tài chính nội bộ và trích dẫn nguồn chính xác. Nhóm nên build Workflow theo pattern RAG: tiền xử lý tài liệu → AI tìm + trích xuất số liệu → tổng hợp câu trả lời kèm trích nguồn → human review. Không nên build phần tự ra quyết định đầu tư hay tự sửa số liệu gốc vì rủi ro quá cao.
```

> Lưu ý: không dùng số liệu AI đưa nếu không verify được link chính thức. Ghi rõ giả định chưa chắc.

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.png/pdf/md`

```text
[1 Nhận câu hỏi: NV phân tích] → [2 Xác định chỉ tiêu cần tra: NV] → [3 Tìm và mở tài liệu: NV] → [4 Trích xuất số liệu — bottleneck: NV] → [5 Tính toán + đối chiếu: NV] → [6 Kiểm chứng kết quả: NV] → [7 Viết câu trả lời + evidence: NV]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | NV phân tích tài chính | Câu hỏi từ quản lý/khách hàng/kiểm toán | Câu hỏi đã hiểu rõ, danh sách chỉ tiêu cần tìm | 3–5 phút, 3–5 câu/ngày | — |
| 2 | NV phân tích tài chính | Câu hỏi đã phân tích | Danh sách chỉ tiêu tài chính cần tra (doanh thu, chi phí, biên LN, kỳ nào) | 3–5 phút | Cần hiểu nghiệp vụ để xác định đúng chỉ tiêu |
| 3 | NV phân tích tài chính | Danh sách chỉ tiêu | Các file/bảng/tài liệu đã mở (Excel, PDF, ERP) | 5–10 phút | Phải nhớ hoặc tìm file nào chứa chỉ tiêu nào |
| 4 | NV phân tích tài chính | Các tài liệu đã mở | Số liệu thô đã trích xuất (ghi ra Excel tạm) | 10–20 phút | **Bottleneck chính**: mở nhiều file, tìm đúng sheet/dòng/cột, dễ nhầm kỳ hoặc đơn vị |
| 5 | NV phân tích tài chính | Số liệu thô | Kết quả tính toán (tỷ lệ, so sánh, xu hướng) | 5–10 phút | Handoff từ trích xuất sang tính toán |
| 6 | NV phân tích tài chính | Kết quả tính toán, số liệu gốc | Kết quả đã kiểm chứng | 5–10 phút | Đối chiếu lại nguồn |
| 7 | NV phân tích tài chính | Kết quả kiểm chứng | Câu trả lời hoàn chỉnh kèm evidence/trích dẫn | 5–10 phút | — |

**Bottleneck chính (2-3 câu):**

```text
Bottleneck nằm ở bước 3–4 (tìm tài liệu + trích xuất số liệu): NV phải nhớ hoặc tìm chỉ tiêu nằm trong file/bảng nào, mở 3–4 file cùng lúc, xác định đúng sheet/dòng/cột/kỳ rồi copy số liệu ra. Hai bước này chiếm 60–70% tổng thời gian (15–30 phút) và là nơi xảy ra sai sót nhiều nhất (nhầm kỳ, nhầm đơn vị, bỏ sót chỉ tiêu).
```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, boundary ở đâu, fallback khi AI sai.

```text
[1 Nhận câu hỏi: NV — người] → [2 AI phân tích câu hỏi + xác định chỉ tiêu: AI — Workflow] → [3 AI truy xuất số liệu từ kho tài liệu (RAG): AI — Workflow] → [4 AI tổng hợp câu trả lời + trích nguồn: AI — Workflow] → [5 NV review + kiểm chứng evidence: người — Boundary] → [6 Gửi câu trả lời: NV — người]

Fallback: Nếu AI không tìm được số liệu hoặc trích nguồn không rõ, NV tự tra cứu thủ công (quay về bước 3–4 cũ). Nếu AI tính sai, NV tự tính lại và ghi nhận case sai để cải thiện pipeline.
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Tổng thời gian | 35 phút/câu hỏi | 10–15 phút/câu hỏi | So sánh thời gian từ nhận câu hỏi đến gửi câu trả lời (log) |
| Số bước | 7 | 6 | Đếm số bước trong workflow |
| Số bước thủ công | 7 (tất cả) | 2 (review + gửi) | Đếm bước cần người thực hiện toàn bộ |
| Bottleneck chính | Tìm tài liệu + trích xuất số liệu (bước 3–4, 15–30 phút) | Review kết quả AI (bước 5, 5–8 phút) | So sánh thời gian bước lâu nhất |
| Risk mới | Không có | AI trích sai số liệu, nhầm kỳ hoặc bịa evidence | Đo bằng tỷ lệ câu trả lời cần sửa số liệu sau review |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | NV phân tích tài chính hoặc kiểm toán viên nội bộ, thường xuyên nhận câu hỏi ad-hoc từ quản lý, khách hàng hoặc cơ quan kiểm toán. Cần tra cứu nhiều nguồn tài liệu (Excel, PDF, ERP) để trả lời chính xác kèm evidence. |
| **Workflow** | Nhận câu hỏi → xác định chỉ tiêu → tìm tài liệu → trích xuất số liệu từ nhiều bảng → tính toán đối chiếu → kiểm chứng → viết câu trả lời kèm evidence. Gồm 7 bước, bước 3–4 thủ công hoàn toàn và tốn thời gian nhất. |
| **Bottleneck** | Bước tìm tài liệu + trích xuất số liệu (bước 3–4) chiếm 60–70% thời gian (15–30 phút/câu). NV phải mở nhiều file, xác định đúng sheet/dòng/cột/kỳ rồi copy ra. Sai sót phổ biến: nhầm kỳ báo cáo, nhầm đơn vị tính. |
| **Impact** | Mỗi câu hỏi mất trung bình 35 phút (baseline từ log 15 câu/2 tuần). Mỗi NV xử lý 3–5 câu/ngày, mất 2–3 giờ/ngày chỉ cho tra cứu + trích xuất. Nếu giảm 50–60% thời gian bước 3–4, tiết kiệm 1–1.5 giờ/ngày/người. |
| **Success Metric** | Giảm thời gian xử lý từ 35 phút xuống dưới 15 phút (baseline: 35 phút từ log). Accuracy số liệu AI ≥ 85% (khớp kiểm chứng thủ công). 100% câu trả lời AI kèm trích nguồn (tên tài liệu, vị trí). |
| **Boundary** | Hệ thống chỉ hỗ trợ tìm số liệu, trích xuất evidence và tổng hợp câu trả lời nháp. Không tự gửi câu trả lời, không ra quyết định tài chính, không sửa dữ liệu gốc. NV bắt buộc review + kiểm chứng + chịu trách nhiệm nội dung cuối. |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ: "Impact" ước tính giảm 50–60% chưa có căn cứ thực nghiệm, là giả định. "Success Metric" yêu cầu ≥ 85% accuracy nhưng chưa định nghĩa rõ đo trên mức nào (đúng số, đúng kỳ, đúng đơn vị, hay tất cả).
- Tôi sửa gì: Bổ sung baseline cụ thể (35 phút từ log 15 câu). Định nghĩa accuracy = số liệu hoàn toàn khớp kiểm chứng thủ công về giá trị + kỳ + đơn vị. Ghi chú 50–60% là giả định sẽ kiểm chứng trong pilot.

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [ ] Thấp (có đúng/sai rõ) / [x] Cao (nhiều cách trả lời vẫn OK) — Vì sao: Cùng một câu hỏi tài chính, có thể trả lời ở nhiều mức chi tiết, dùng nhiều cách trích dẫn evidence đều hợp lệ. Đáp án phụ thuộc ngữ cảnh và người hỏi.
- Độ phức tạp: [ ] Thấp (1-2 bước) / [x] Cao (3+ bước/nguồn, phụ thuộc nhau) — Vì sao: Cần truy xuất 3+ nguồn tài liệu, xác định chỉ tiêu, trích số liệu đúng kỳ, tính toán và đối chiếu. Các bước phụ thuộc nhau — không tính được nếu chưa trích đúng số.

**Bài toán nhóm nằm ở ô nào:**

```text
Ô "Cao – Cao" (Mơ hồ cao + Phức tạp cao) → phù hợp nhất với Workflow (có thể tiến tới Agent nếu cần tự chọn tài liệu).
```

**Vì sao (2-3 câu):**

```text
Bài toán yêu cầu truy xuất từ nhiều nguồn tài liệu có cấu trúc khác nhau (Excel, PDF, database), xác định đúng chỉ tiêu và kỳ, rồi tổng hợp thành câu trả lời có evidence — không thể giải bằng Rule cứng. Tuy nhiên, pipeline vẫn tuần tự (phân tích → truy xuất → tổng hợp → trích nguồn) nên Workflow là đủ, chưa cần Agent tự lập kế hoạch. NV có thể chỉ định phạm vi tài liệu cần tra.
```

### 6.1. So sánh Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | Dùng keyword matching / lookup table để tra chỉ tiêu trong bảng có cấu trúc cố định (VD: tra doanh thu Q1/2024 trong file tổng hợp). | Đủ khi câu hỏi đơn giản, chỉ tra 1 chỉ tiêu/1 bảng/1 kỳ. | Không xử lý được câu hỏi so sánh nhiều kỳ, tính tỷ lệ, hoặc tổng hợp đa nguồn. Phải cập nhật rule khi thêm tài liệu. | Dùng cho **bước tiền xử lý**: chuẩn hóa tên chỉ tiêu, mapping kỳ báo cáo, validate format. |
| **Workflow** | Pipeline: (1) LLM phân tích câu hỏi → xác định chỉ tiêu + kỳ, (2) RAG truy xuất đoạn tài liệu liên quan, (3) LLM trích xuất số liệu + tính toán, (4) LLM tổng hợp câu trả lời kèm trích nguồn, (5) Human review. Mỗi bước có prompt và output format rõ. | Đủ khi phạm vi tài liệu đã index trước và câu hỏi phân tích qua prompt được — tức phần lớn câu hỏi ad-hoc thường gặp. | LLM có thể trích sai số liệu từ bảng phức tạp hoặc nhầm kỳ. RAG có thể trả về đoạn không liên quan nếu embedding bảng số kém. | **Chọn** — Dùng cho **bước 2-4** (phân tích + truy xuất + tổng hợp). |
| **Agent** | Agent tự quyết định cần tra tài liệu nào, tự gọi tool đọc file/query database, tự chọn chiến lược tính toán và tự kiểm chứng trước khi đưa câu trả lời. | Cần khi câu hỏi rất phức tạp, đòi hỏi nhiều vòng tra cứu hoặc không biết trước cần tài liệu nào. | Khó kiểm soát, có thể truy cập sai tài liệu hoặc tính sai mà không có human checkpoint. Chi phí cao, khó debug. | Không chọn ở giai đoạn này — NV chỉ định phạm vi tài liệu. Có thể nâng cấp sau khi Workflow ổn định. |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. Rule có giải được 70-80% case không? → Không. Phần lớn câu hỏi cần tra nhiều nguồn, so sánh nhiều kỳ, tính tỷ lệ — vượt lookup table. Rule chỉ giải khoảng 20–30% case đơn giản.
2. Các bước có đi thẳng một đường không hay phải rẽ nhánh? → Cơ bản đi thẳng: phân tích → truy xuất → tổng hợp → review. Có thể loop lại truy xuất nếu thiếu dữ liệu, nhưng flow chính tuyến tính, phù hợp Workflow.
3. Có thật sự cần Agent tự lập kế hoạch + gọi tool không? → Chưa cần ở pilot. NV chỉ định phạm vi tài liệu. Agent phù hợp khi scale kho tài liệu rất lớn, nhưng pilot nên dùng Workflow để dễ kiểm soát.
4. Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu? → NV phân tích (người chuyên môn) phát hiện ở bước review bằng cách click trích nguồn đối chiếu tài liệu gốc. Sửa mất 5–10 phút.
5. Có hạ được từ Agent → Workflow → Rule không? → Đã hạ từ Agent xuống Workflow. Không hạ tiếp xuống Rule vì cần LLM để phân tích câu hỏi tự nhiên, truy xuất ngữ nghĩa và tổng hợp câu trả lời kèm evidence.

**Mức chọn:**

```text
Workflow
```

**Vì sao chọn (3-4 câu):**

```text
Workflow phù hợp nhất vì pipeline tuần tự rõ ràng (phân tích → truy xuất → trích xuất → tổng hợp kèm nguồn), đầu vào xác định (kho tài liệu đã index) và output format ổn định. LLM + RAG cần thiết để hiểu câu hỏi tự nhiên và truy xuất ngữ nghĩa từ kho tài liệu — Rule không làm được. Tuy nhiên chưa cần Agent vì NV chỉ định phạm vi tài liệu, không cần AI tự khám phá. Workflow cũng cho phép bắt buộc trích nguồn ở mỗi bước, dễ kiểm chứng và debug hơn Agent.
```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text
Rule chỉ tra lookup table cố định (1 chỉ tiêu, 1 kỳ, 1 bảng), không phân tích câu hỏi tự nhiên, không truy xuất ngữ nghĩa và không tổng hợp câu trả lời kèm evidence từ nhiều nguồn. Khoảng 70–80% câu hỏi tài chính ad-hoc cần so sánh nhiều kỳ hoặc tổng hợp từ 2+ nguồn — bắt buộc cần LLM và retrieval.
```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | NV phân tích tài chính / kiểm toán viên nội bộ (1–5 năm KN), xử lý 3–5 câu hỏi ad-hoc/ngày từ quản lý, khách hàng hoặc cơ quan kiểm toán. Có quyền truy cập kho tài liệu tài chính nội bộ. |
| **Workflow** | (1) NV nhận câu hỏi → (2) AI phân tích câu hỏi, xác định chỉ tiêu + kỳ (Workflow) → (3) AI truy xuất số liệu qua RAG (Workflow) → (4) AI tổng hợp câu trả lời kèm trích nguồn (Workflow) → (5) NV review + kiểm chứng evidence (Boundary) → (6) Gửi câu trả lời. |
| **Bottleneck** | Bước 3–4 current workflow (tìm tài liệu + trích xuất) chiếm 60–70% thời gian (15–30 phút/câu), phải mở 3–4 file, xác định đúng sheet/dòng/cột/kỳ. Sai sót phổ biến: nhầm kỳ, nhầm đơn vị. |
| **Impact** | Giảm thời gian xử lý từ 35 phút xuống dưới 15 phút/câu (baseline: 35 phút từ log 15 câu/2 tuần). Tiết kiệm 1–1.5 giờ/ngày/người cho 3–5 câu hỏi ad-hoc. |
| **Success Metric** | Thời gian xử lý ≤ 15 phút/câu (baseline: 35 phút). Accuracy số liệu ≥ 85% (khớp giá trị + kỳ + đơn vị). 100% câu trả lời AI kèm trích nguồn (tên tài liệu, vị trí). |
| **Boundary** (làm / không làm) | **Làm**: Phân tích câu hỏi, truy xuất số liệu từ kho đã index, tổng hợp câu trả lời nháp kèm trích nguồn. **Không làm**: Tự gửi câu trả lời, tự ra quyết định tài chính, truy cập hệ thống giao dịch, sửa dữ liệu gốc. |
| **AI intervention point** (can thiệp sau bước nào, trước bước nào) | Can thiệp sau bước 1 (nhận câu hỏi) và trước bước 5 (review của NV). AI thực hiện bước 2–4: phân tích câu hỏi → truy xuất qua RAG → tổng hợp câu trả lời kèm nguồn. |
| **Mức chọn** (Rule / Workflow / Agent + 1 câu vì sao) | Workflow — pipeline tuần tự với đầu vào xác định (kho tài liệu đã index), cần LLM + RAG nhưng không cần Agent tự lập kế hoạch. |
| **Rủi ro & người thật kiểm tra** (rủi ro lớn nhất + ai kiểm tra bằng cách nào) | Rủi ro lớn nhất: AI trích sai số liệu (nhầm kỳ, nhầm chỉ tiêu) hoặc bịa evidence. NV phân tích kiểm tra bằng cách click trích nguồn đối chiếu tài liệu gốc. Nếu sai, NV tự tra lại và ghi nhận case để cải thiện pipeline. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | Yes | Actor là NV phân tích tài chính/kiểm toán, workflow 6 bước (future) có rõ đầu vào, đầu ra, thứ tự và người/AI từng bước. |
| Baseline + metric đo được chưa? | Yes | Baseline 35 phút/câu từ log (15 mẫu/2 tuần). Metric: thời gian, accuracy số liệu, tỷ lệ có trích nguồn — đều đo được trong lab. |
| Data/input đủ dùng chưa? | Yes | Nhóm có thể tạo bộ tài liệu mẫu từ BCTC công khai của công ty niêm yết (cafef.vn, vietstock.vn). Tạo 10–15 câu hỏi mẫu có đáp án chuẩn. |
| AI sai, hậu quả chấp nhận được không? | Yes | NV bắt buộc review + kiểm chứng trước khi gửi. Hậu quả tối đa là mất thêm 5–10 phút sửa. Trong lab không có rủi ro tài chính thực tế. |
| Có người review/owner không? | Yes | NV phân tích tài chính (người chuyên môn) review bằng cách đối chiếu trích nguồn AI với tài liệu gốc. |
| Có cách non-AI đơn giản hơn không? | No | Dashboard/BI giải quyết câu hỏi chuẩn nhưng không xử lý ad-hoc đa nguồn. Macro/VBA chỉ hoạt động trong 1 file, không truy xuất ngữ nghĩa liên file. |

**Decision:**

```text
Go
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text
Bài toán có actor rõ (NV phân tích tài chính), workflow đã validate qua interview (3 người) và survey (6 người) với baseline đo được (35 phút/câu từ log 15 mẫu). Nhóm có thể tạo bộ dữ liệu mẫu từ BCTC công khai để chạy pilot ngay. Rủi ro khi AI sai chấp nhận được vì NV bắt buộc review + kiểm chứng — trong lab không có rủi ro tài chính thực tế. Pattern RAG đã chứng minh hiệu quả cho bài toán truy xuất thông tin từ kho tài liệu.
```

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text
Data: Tạo kho 5–10 tài liệu tài chính mẫu (BCKQKD, bảng CĐKT, báo cáo LCTT) từ 2–3 công ty niêm yết (cafef.vn). Chuẩn bị 10 câu hỏi có đáp án chuẩn. Chạy tay: paste tài liệu + câu hỏi vào ChatGPT/Claude với prompt yêu cầu trả lời kèm trích nguồn. Đo 3 số: (1) Thời gian từ nhận câu hỏi đến câu trả lời — so baseline 35 phút, (2) Accuracy số liệu (khớp đáp án về giá trị + kỳ + đơn vị) — mục tiêu ≥ 85%, (3) Tỷ lệ có trích nguồn đầy đủ — mục tiêu 100%.
```

**Nếu Not Yet — cần validate gì trước:**

```text
—
```

**Nếu No-Go — làm gì thay AI:**

```text
—
```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text
Dừng AI nếu sau 10 câu hỏi pilot, accuracy số liệu < 70% hoặc thời gian tổng (chạy AI + review + sửa) không giảm ít nhất 30% so với thủ công. Khi đó quay về cách cũ: NV tra cứu thủ công, chỉ giữ bước Rule chuẩn hóa tên chỉ tiêu và mapping kỳ báo cáo.
```

---

### Self-check nộp phần 02 (nhóm)
- [x] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score)
- [x] Có validation (quote thật) + research (link kiểm được)
- [x] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [x] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [x] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do
