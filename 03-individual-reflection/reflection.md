# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Đặng Quang Hưng
- Mã học viên: 2A202602719
- Nhóm: Nhóm 6 thành viên (Mai Văn Trường, Hồ Ngọc Mai, Vũ Quốc Huy, Nguyễn Hoàng Cường, Nguyễn Hữu Thành, Đặng Quang Hưng)
- Candidate problem nhóm chọn: #12 — Trả lời câu hỏi tài chính phức tạp từ nhiều bảng và tài liệu

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Đóng góp 3 candidate problems thuộc domain Giáo dục/TA (Chuẩn hóa báo cáo tiến độ học viên, Rà soát lỗi IELTS lặp lại, Trả lời thắc mắc ngoài giờ). | Bổ sung cho nhóm các góc nhìn về bài toán tốn thời gian ở khâu phản hồi và tạo nhận xét sư phạm. |
| Pitch Problem Card | Pitch candidate #1 (Chuẩn hóa báo cáo tiến độ học viên), phân tích chi tiết bottleneck ở bước chuyển ghi chú thô thành nhận xét cá nhân hóa. | Giúp nhóm hiểu rõ cách phân tích một bottleneck từ 60% thời gian chấm bài/nhận xét. |
| Challenge bài của bạn khác | Challenge candidate #14 (gán thẻ ticket) về thiếu dữ liệu CSKH thực tế và candidate #5 (nhắc deadline) vì có thể dùng Rule/Reminder đơn giản mà chưa cần AI. | Giúp nhóm loại bỏ các bài toán chưa đủ dữ liệu hoặc có thể giải quyết bằng giải pháp non-AI đơn giản. |
| Chọn candidate problem | Chấm điểm 3 shortlist candidates (#7, #14, #12), phân tích vì sao bài #12 có impact lớn nhất và phù hợp với RAG + Workflow. | Thống nhất được candidate duy nhất (#12) đạt điểm cao nhất (34/35 điểm). |
| Rule / Workflow / Agent | Đánh giá ma trận Mơ hồ (Cao) - Phức tạp (Cao), phản biện nhóm hạ từ Agent xuống Workflow để dễ kiểm soát rủi ro. | Thống nhất chọn mức Workflow (LLM + RAG), tránh phức tạp hóa bài toán ở giai đoạn pilot. |
| Decision | Thống nhất quyết định Go, thiết kế kịch bản pilot nhỏ (10-15 câu hỏi từ BCTC công khai) và đưa ra điều kiện Exit/Rollback rõ ràng. | Chốt được kế hoạch triển khai pilot thực tế và phương án an toàn khi AI không đạt kỳ vọng. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Dấu tay rõ nhất của tôi là việc phản biện để nhóm chọn mức Workflow thay vì Agent hào nhoáng, đồng thời thiết kế chi tiết tiêu chuẩn đo lường Accuracy (phải khớp cả giá trị, kỳ báo cáo, đơn vị tính) và quy định bắt buộc AI phải trích dẫn nguồn đến từng sheet/dòng/cột trước khi human review.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Problem Card | Dùng AI hỗ trợ dựng draft workflow 5 bước current/future cho Problem Card cá nhân. | Bóc tách nhanh cấu trúc workflow tuyến tính và đề xuất cách viết bottleneck ngắn gọn. | Thiết kế workflow quá lý tưởng, thiếu bước kiểm tra lại (human check) và không có fallback khi AI sai. | Thêm bước Fallback thủ công và gắn nhãn Boundary rõ ràng cho bước người review. |
| Workflow | Dùng AI phân rã input/output chi tiết từng bước cho Current và Future Workflow. | Đề xuất khung thông tin đầy đủ gồm Actor, Input, Output và thời gian cho mỗi bước. | Bỏ qua bước trích dẫn nguồn gốc (citation) của dữ liệu tài chính, cho rằng AI có thể tự trả lời luôn. | Bổ sung bắt buộc yêu cầu AI phải output kèm trích dẫn (tên file, sheet, dòng, cột) ở bước 4. |
| Rule / Workflow / Agent | Dùng AI phân tích bài toán theo ma trận độ mơ hồ vs độ phức tạp để chọn kiến trúc. | Gợi ý khung lý thuyết đánh giá độ mơ hồ (Cao) và độ phức tạp (Cao). | Xu hướng đẩy bài toán lên mức Agent (tự động truy vấn database, tự lập kế hoạch) quá phức tạp và đắt đỏ. | Hạ xuống mức Workflow (LLM + RAG có hướng dẫn), giữ việc chọn phạm vi tài liệu cho người dùng. |
| Decision | Dùng AI brainstorm các chỉ số đo lường cho pilot và các kịch bản rollback. | Gợi ý cấu trúc các con số cần đo trong pilot (thời gian, accuracy, citation rate). | Đề xuất kịch bản pilot quá cồng kềnh với dữ liệu doanh nghiệp thật vốn khó tiếp cận ngay. | Sửa kịch bản pilot thành sử dụng 10-15 câu hỏi mẫu trên BCTC công khai của các công ty niêm yết (cafef.vn). |

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
Khi cùng nhóm trải qua các phase từ phân tích problem cá nhân đến đưa ra quyết định cuối cùng, bài học lớn nhất mà tôi rút ra được là việc giữ cho tư duy luôn bám sát vào workflow thực tế thay vì bị cuốn theo các giải pháp công nghệ hào nhoáng. Khi thảo luận ở Phase 6, nhóm đã có lúc rơi vào bẫy 'solution-first' khi một số thành viên muốn xây dựng một Autonomous Agent tự động truy cập kho dữ liệu và tự lập kế hoạch tra cứu cho ngầu. Tuy nhiên, sau khi phân tích kỹ ma trận độ phức tạp và boundary, tôi đã cùng nhóm tỉnh táo hạ mức độ xuống Workflow (LLM kết hợp RAG) vì nhận thấy người dùng hoàn toàn có thể chỉ định phạm vi tài liệu, còn AI chỉ nên tập trung vào việc tìm kiếm, trích xuất và tổng hợp câu trả lời kèm trích dẫn nguồn. Đối với tôi, điều khó nhất khi hoàn thiện Problem Statement không phải là định xuất thời gian mà là thiết lập Boundary nghiêm ngặt. Dấu tay rõ nhất của tôi trong artifact cuối nằm ở việc thiết kế tiêu chuẩn đo lường Accuracy chi tiết (phải khớp cả giá trị, kỳ báo cáo và đơn vị tính) cùng quy tắc 100% câu trả lời của AI bắt buộc phải kèm trích nguồn chính xác đến từng dòng, cột. Nếu được làm lại từ đầu, tôi sẽ challenge nhóm mạnh hơn ngay từ bước Quick Validation về việc thu thập log dữ liệu thực tế sớm hơn để tránh mất thời gian tranh luận dựa trên các giả định chủ quan.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI

