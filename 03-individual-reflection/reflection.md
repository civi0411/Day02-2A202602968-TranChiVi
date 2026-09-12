# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Trần Chí Vĩ
- Mã học viên: 2A202602968
- Nhóm: Nhóm Lab Day 02 (6 thành viên)
- Candidate problem nhóm chọn: Actionable Math & Engineering Spec Sheet Extraction for Technical Papers (Tóm tắt có cấu trúc & Trích xuất Thuật toán / Thông số Kỹ thuật từ Bài báo Khoa học 15–20 trang).

---

## 1. Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Lọc các vấn đề đau đầu nhất khi làm QuantAINexus và chuẩn bị Seminar tại KHTN. Cung cấp danh sách 8 bài toán, chốt lại Problem Card liên quan đến bóc tách công thức toán từ paper. | Đưa ra danh sách bài toán có số đo thời gian thực tế rõ ràng, phản ánh đúng "nỗi đau" cạn kiệt trí lực. |
| Pitch Problem Card | Pitch Card #1 trong 2 phút, chỉ rõ 2 bottleneck: 60 phút giải mã toán học và 35 phút lùng sục thông số kỹ thuật. | Giúp nhóm thấy rõ tính lặp lại (weekly) và cạn kiệt năng lượng kéo dài gây đình trệ code. |
| Challenge bài của bạn khác | Phản biện rủi ro bảo mật dữ liệu của bài "Tóm tắt Group Chat" (Quân) và rào cản dataset hình ảnh của bài "Review CV" (Tuấn). | Nhóm nhận ra cần tập trung vào bài toán có tính an toàn dữ liệu cao (như PDF học thuật public). |
| Gom trùng / cluster | Đề xuất gộp ý tưởng số #1 của tôi (giải mã toán học) và ý #8 của Tuấn (bóc tách technical config) thành cụm "Trích xuất & Tóm tắt Tri thức Kỹ thuật". | Tạo ra một candidate hoàn hảo, có độ phủ 100% các thành viên kỹ thuật trong nhóm. |
| Chọn candidate problem | Cung cấp luận điểm về tính lặp lại và tính logic chặt chẽ của ký hiệu toán học có thể dùng AI bóc tách tốt. | Nhóm đồng thuận chấm 34 điểm cho candidate "Math & Engineering Spec Sheet" để làm bài toán chính. |
| Validation / research | Trực tiếp tham gia phỏng vấn 1 bạn AI Intern, khảo sát 12 kỹ sư và đưa ra đối chuẩn (benchmark) với Elicit, NotebookLM. | Chứng minh tính khả thi thực tế và làm rõ sự khác biệt của giải pháp nhóm so với Chatbot Q&A thông thường. |
| Workflow nhóm | Thiết kế kiến trúc 4 bước phân định rạch ròi: Rule (Parser) → AI (LLM) → Human (Audit) → Downstream. | Giúp workflow giảm tổng thời gian từ 145' xuống 35', cắt giảm hoàn toàn sự cạn kiệt nhận thức. |
| Problem Statement | Viết field Boundary cực chặt chẽ và thiết lập Success Metric đạt độ chính xác ≥90% đối chiếu 1-1. | Đảm bảo Problem Statement v1 của nhóm cực kỳ sắc bén, không rơi vào bẫy "AI giải quyết mọi thứ". |
| Rule / Workflow / Agent | Phân tích ma trận Fit Matrix và bảo vệ quyết định chốt mức AI Workflow thay vì Agent. | Giúp nhóm tránh bẫy "solution-first", loại bỏ rủi ro Agent tự chạy code sinh ra hệ quả sai lệch. |
| Decision | Đặt ra kịch bản Rollback khắt khe: Nếu AI sai >15% hoặc chạy >10 phút thì dừng ngay lập tức. | Giúp quyết định GO an toàn tuyệt đối, có exit plan rõ ràng để rà soát. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**
Với vai trò Facilitator và Tech Lead, "dấu tay" đậm nét nhất của tôi là việc kiến trúc hệ thống **AI-Assisted Spec Extraction** kết hợp **Human Audit Boundary 20 phút** bắt buộc, đồng thời ép AI phải đính kèm *link citation trỏ trực tiếp về số trang PDF gốc*, chặn đứng triệt để nỗi lo "ảo giác toán học" của nhóm.

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Dùng AI đóng vai trò "Devil's Advocate" phản biện các pain points cá nhân. | AI chỉ ra thiếu sót về việc các pain point ban đầu mang tính định tính. | AI gợi ý một số bài toán vĩ mô chung chung thiếu căn cứ thực tiễn. | Tự loại bỏ các bài toán mơ hồ, bổ sung thời gian bấm giờ thực tế (145 phút/paper) vào bài toán cuối. |
| Problem Card | Xin AI gợi ý phân rã các chặng đọc paper khoa học. | Giúp liệt kê được các thuật ngữ kỹ thuật trong một quy trình đọc paper chuẩn. | AI vẽ ra 10 bước rườm rà, quá lý thuyết đối với một kỹ sư thực chiến. | Tự cô đọng lại thành 5 bước sát thực tế: Abstract, Methodology, Config, và Synthesize. |
| Workflow | Gợi ý code Mermaid/ASCII text GUI cho quy trình Future State. | Định dạng sơ đồ Before/After (thời gian, diễn giải) sạch sẽ, cực kỳ trực quan. | AI phân bổ thời gian Human check quá lạc quan (chỉ 2 phút). | Ép lại thời gian chốt chặn Human Boundary là 20 phút để sát với tính chuyên môn sâu. |
| Research | Hỏi AI về các tool tóm tắt paper hiện hành trên thị trường. | Gợi ý tên các nền tảng lớn như Elicit, Consensus, NotebookLM. | AI khuyên dùng NotebookLM là đủ để thay thế hoàn toàn việc đọc. | Nhận định Chatbot thiếu Schema chuẩn, tôi tự đổi hướng sang dùng Math Parser + LLM JSON cấu trúc cứng. |
| Problem Statement | Phản biện tính chặt chẽ của Problem Statement v0. | Ghi nhận thiếu sót ở field Boundary chưa làm rõ phạm vi "Không làm". | AI viết Boundary lan man về đạo đức AI và bản quyền. | Chặt gọn thành ranh giới hành động kỹ thuật: "Không tự chốt slide, không tự code PoC". |
| Rule / Workflow / Agent | Xin gợi ý tranh biện giữa độ phân giải giải pháp (Agent vs Workflow). | Chỉ ra rõ ưu nhược điểm kỹ thuật của từng mức độ tự động hóa. | AI cố gắng thuyết phục nên dùng Autonomous Agent để trông "pro" hơn. | Loại bỏ hoàn toàn Agent để giữ an toàn kỹ thuật, chốt mức Workflow tuyến tính dễ kiểm soát. |
| Decision | Sinh kịch bản Exit Plan và Success Metrics cho Pilot. | Gợi ý các tiêu chí cơ bản để đánh giá thành công của dự án AI. | AI không định lượng rõ rệt các con số để đưa ra quyết định Rollback. | Tự ép số liệu cứng: Lỗi >15% (Critical unsupported claim) thì Rollback về manual ngay. |

---

## 3. Reflection câu hỏi mở

**Reflection:**

Trong suốt quá trình thực hiện Lab 02, điều tôi thấm thía nhất chính là bài học "Problem-first, not AI-first". Ban đầu, khi thiết kế framework cho QuantAINexus, tôi bị cuốn vào tham vọng xây dựng một "Autonomous AI Agent" có thể tự đọc tài liệu FinWorld, tự dịch công thức và tự chạy code. Tuy nhiên, khi đào sâu vào điểm nghẽn 145 phút đọc paper – nơi cạn kiệt trí lực thực sự diễn ra, tôi nhận ra AI tự trị là một "cái bẫy" nguy hiểm. Nếu phó mặc hoàn toàn cho Agent, rủi ro AI ảo giác (hallucinate) các tham số tensor hay dấu của phương trình ma trận có thể làm hỏng toàn bộ pipeline chiến lược giao dịch phía sau. 

Khoảnh khắc nhóm bừng sáng nhất là khi tôi đề xuất gom ý tưởng "giải mã toán học" của mình với ý tưởng "bóc tách cấu hình triển khai" của Minh Tuấn thành một bài toán duy nhất: **Actionable Math & Engineering Spec Sheet**. Việc áp dụng Ma trận độ phù hợp (Fit Matrix) đã giúp tôi dũng cảm "hạ cấp" giải pháp xuống mức **AI Workflow**, trong đó máy làm đúng việc parser, AI làm đúng việc trích xuất JSON Schema, và chốt chặn quan trọng nhất là **Human Audit Boundary 20 phút** kèm citation số trang gốc. Thiết kế này không hề làm giảm "độ ngầu" của sản phẩm, ngược lại, nó mang tính ứng dụng (actionable) và an toàn cực cao cho những người nghiên cứu thực chiến. 

Dấu tay lớn nhất của tôi nằm ở sự quyết liệt từ chối Chatbot Q&A tự do, bắt buộc thiết kế một Workflow tuyến tính có exit plan rõ ràng. Nếu được làm lại, tôi sẽ thúc đẩy việc phỏng vấn đối chuẩn (benchmark) sâu hơn ngay từ Phase 3 để quá trình chốt hạ Candidate diễn ra thậm chí còn nhanh gọn và sắc bén hơn nữa.

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
