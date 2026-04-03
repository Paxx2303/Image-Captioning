# Assignment 2

---

## (1) Sang Phan

**Context**: Một AI Engineer làm việc ở công ty phần mềm và các công việc gặp phải

**Bài toán:** Lặp lại → Update requirements.txt và test dependencies sau mỗi PR merge cho LangChain/OpenAI.

### Challenge & Trả lời

| Câu challenge | Trả lời |
|:---|:---|
| "Rule/script đủ chưa? Có thật sự cần AI không?" | "Script automation (như Dependabot) đủ cho update basic dependencies. Nhưng với LangChain/OpenAI, cần AI để detect breaking changes trong code logic, không chỉ version conflicts — rule không đủ cho complex integrations." |
| "Ngoài bạn, ai đau nữa? Bao nhiêu người?" | "Team AI Engineer có 5 người, tất cả đều gặp pain này sau mỗi PR merge. DevOps team cũng bị impact khi phải rollback nếu test fail." |
| "Metric đo được không? Có số cụ thể chưa?" | "Có — thời gian update từ 45 min xuống dưới 10 min. Tỉ lệ test failures từ 20% xuống dưới 5%. Số PR delays giảm từ 3/tuần xuống 0." |

### Cards bị loại

| Cards bị loại | Lý do |
|:---|:---|
| #2 — Debug Agent | Technical nhưng scope hẹp, rule/script đủ |
| #5 — Integrate Azure AI Search | Collaboration issue, AI giúp nhưng human sync cần |

**Vote: 6/7**

---

## (2) Nam

**Bài toán:** Tổng hợp dữ liệu từ database để làm các báo cáo định kỳ, tốn nhiều thời gian

### Challenge & Trả lời

| Câu hỏi Challenge | Trả lời chi tiết |
|:---|:---|
| Hiện tại bạn đang mất bao nhiêu thời gian để tổng hợp dữ liệu từ database cho mỗi báo cáo định kỳ, và con số đó chiếm bao nhiêu % tổng thời gian làm việc của bạn trong tuần? | Mỗi báo cáo tháng mất khoảng **6–8 tiếng**: 2 tiếng export data từ 3 nguồn (ERP, CRM, Excel phòng ban), 3 tiếng clean và chuẩn hóa format, 2 tiếng tổng hợp vào template. Tổng cộng chiếm khoảng **15–20%** thời gian làm việc cả tuần (chưa tính báo cáo quý). |
| Điều gì xảy ra nếu dữ liệu từ các nguồn không khớp nhau khi tổng hợp — bạn xử lý như thế nào và mất thêm bao lâu? | Khi số liệu lệch nhau giữa các nguồn phải quay lại hỏi từng phòng ban để xác nhận, trung bình mất thêm **2–3 tiếng** email qua lại. Đôi khi phát hiện lúc sắp deadline nên phải làm overtime. Chưa có quy trình chuẩn để xác định nguồn nào là "source of truth" nên mỗi lần xử lý khác nhau. |
| Nếu có một hệ thống tự động kéo dữ liệu từ tất cả các nguồn và tạo sẵn báo cáo, bạn sẽ dùng thời gian tiết kiệm được để làm gì — và điều đó có giá trị hơn việc tổng hợp thủ công không? | Nếu tiết kiệm được 6–8 tiếng mỗi tháng, thời gian đó sẽ dùng để phân tích sâu hơn vào nguyên nhân biến động số liệu và đưa ra khuyến nghị cho ban lãnh đạo. Giá trị cao hơn nhiều vì đây là phần tạo ra quyết định kinh doanh thực sự, thay vì chỉ copy số từ chỗ này sang chỗ khác. |

### Cards bị loại

| Card bị loại | Lý do |
|:---|:---|
| #1 Tổng hợp dữ liệu để làm các báo cáo định kỳ | Khó đo quality improvement, metric yếu hơn |
| #3 Sắp xếp lịch trình cho tổ chức | Khó đo quality improvement, metric yếu hơn |

**Vote: 6/7**

---

## (3) Dũng

**Bài toán (AI can do better):** Up bài trên group hoặc confession của trường để xin tài liệu hoặc review môn học nhằm lựa chọn học phần và giảng viên

### Challenge & Trả lời

| Câu hỏi Challenge | Trả lời chi tiết |
|:---|:---|
| "Hiện tại bạn đang làm gì để tìm tài liệu, review môn học và chọn giảng viên?" | Mình thường up bài hỏi trên group lớp, group ngành hoặc confession của trường để xin tài liệu và review môn học, giảng viên. |
| "Bạn mất bao nhiêu thời gian và gặp những khó khăn gì khi làm theo cách này?" | Phải chờ mọi người trả lời, đôi khi không ai rep hoặc thông tin sai, thiếu. Phải hỏi nhiều group khác nhau, tốn thời gian lọc thông tin và đôi khi vẫn không tìm được review đáng tin cậy. |
| "Nếu có một hệ thống AI tự động tổng hợp review môn học, giảng viên từ nhiều nguồn (group, confession, feedback cũ…) và đưa ra đánh giá khách quan, bạn sẽ dùng nó không? Tại sao?" | Mình có, vì sẽ tiết kiệm rất nhiều thời gian, thông tin đầy đủ và khách quan hơn và mình có thể so sánh dễ dàng giữa các môn và giảng viên để chọn học phần phù hợp với mục tiêu và khả năng của bản thân. |

### Cards bị loại

| Card bị loại | Lý do |
|:---|:---|
| **1 - Quản lý lưu lượng truy cập đăng kí tín chỉ** | Khó xử lý khả năng phân phối lưu lượng truy cập theo băng thông |
| **2 - Quản lý thông tin từ đa nguồn communication channel** | Bài toán có tính riêng tư cao (Privacy), khó truy cập dữ liệu tin nhắn để huấn luyện AI. Ngoài ra có thể giải quyết một phần bằng các công cụ ghim/nhắc lịch thủ công. |

**Vote: 5/7**

---

## (4) Ánh

**Bài toán:** Đề xuất phương tiện di chuyển khả dụng + nhanh + rẻ dựa vào thu thập dữ liệu của các app Grab, Xanh, Be

### Challenge & Trả lời

| Câu challenge | Trả lời của Ánh |
|:---|:---|
| "Chỉ cần mở app xem là xong, có thực sự cần AI không? Rule/script so sánh giá bình thường có đủ chưa?" | "Nếu chỉ so sánh giá hiện tại thì script đủ. Nhưng AI cần để dự báo thời gian tài xế đến dựa trên dữ liệu lịch sử và tình trạng kẹt xe real-time, đồng thời học hỏi thói quen của người dùng (ưu tiên rẻ hay ưu tiên nhanh) để đưa ra đề xuất thông minh nhất." |
| "Vấn đề này ngoài bạn ra còn ai đau nữa không?" | "Tất cả sinh viên và nhân viên văn phòng di chuyển bằng app hàng ngày. Đặc biệt là cư dân Vin thường xuyên ưu tiên Xanh SM nhưng vẫn muốn cân đối giá với các bên khác." |
| "Metric đo được không? Có số cụ thể chưa?" | "Có — Giảm thời gian chọn app từ 5 phút xuống < 30 giây. Giảm chi phí di chuyển hàng tháng trung bình 15-20% nhờ luôn chọn được deal rẻ nhất." |
| "Có đảm bảo truy xuất được thông tin xe, giá tiền, khuyến mãi.. từ các ứng dụng đặt xe khác như Grab/Be/Xanh SM.. không?" | "Có — hệ thống hoàn toàn có thể truy xuất dữ liệu giá tiền và khuyến mãi từ các nền tảng như Grab, Be và Xanh SM thông qua các hình thức tích hợp chính thức." |

### Cards bị loại

| Card bị loại | Lý do |
|:---|:---|
| #1 Tính Calo, đề xuất khẩu phần ăn chuẩn dinh dưỡng | Độ chính xác cao, khó validate trong scope lab và phụ thuộc dữ liệu y tế chuyên sâu vượt quá phạm vi MVP |
| #3 Hỗ trợ đọc tài liệu | Khó đo mức độ hiểu, rủi ro sai nội dung và thiếu trust nên không giải quyết triệt để pain |

**Vote: 7/7**

---

## (5) Thái

**Bài toán:** Dự đoán trạng thái thực tế của trụ sạc VinFast cho cư dân

### Phase 3 — PITCH-CHALLENGE-VOTE

**Thái pitch Card #3 cho nhóm (2 min):**

> "Tôi là cư dân Vin và đang dùng xe điện. Vấn đề lớn nhất hiện nay không phải là thiếu trạm sạc, mà là trạm sạc ảo (Ghosting): app báo trống nhưng đến nơi thì trụ hỏng hoặc bị xe khác chiếm chỗ. Tôi muốn dùng AI để dự báo 'Độ tin cậy' của trạm sạc đó trước khi người dùng bắt đầu di chuyển, giúp họ không bị lãng phí 20-30 phút đi tìm trạm mới."

### Challenge & Trả lời

| Câu challenge | Trả lời của Thái |
|:---|:---|
| **"Tại sao không dùng hệ thống báo hỏng thủ công? Cần gì AI?"** | "Báo hỏng thủ công luôn có độ trễ lớn. AI có thể phân tích **mẫu dữ liệu (patterns)**: nếu một trụ sạc không có giao dịch phát sinh trong 3 tiếng dù app báo trống, AI sẽ tự suy luận khả năng cao trụ đó đang hỏng hoặc bị chiếm chỗ và hạ điểm uy tín của trạm đó xuống." |
| **"Dữ liệu ở đâu để dự báo chính xác?"** | "Chúng ta có dữ liệu từ **lịch sử giao dịch sạc**, dữ liệu **log của trụ sạc** gửi về server (IoT) và báo cáo từ cộng đồng cư dân. AI sẽ kết hợp các nguồn này để đưa ra chỉ số xác suất thực tế." |
| **"Metric thành công là gì? Làm sao biết AI của bạn tốt hơn hệ thống hiện tại?"** | "Metric chính là **Tỷ lệ sạc thành công ngay lần đầu**. Hiện tại có thể chỉ đạt 70%, mục tiêu của AI là đẩy con số này lên **> 95%**, giảm thiểu tối đa số lần khách phải di chuyển sang trạm thứ hai." |

### Cards bị loại

| Card bị loại | Lý do |
|:---|:---|
| **#1 — Lý thuyết lái xe** | Vòng đời sử dụng ngắn (thi xong là bỏ). Tính cá nhân hóa cao nhưng giá trị kinh tế thấp hơn bài toán trạm sạc. |
| **#2 — Quản lý nhóm chat** | Bài toán có tính riêng tư cao (Privacy), khó truy cập dữ liệu tin nhắn để huấn luyện AI. Ngoài ra có thể giải quyết một phần bằng các công cụ ghim/nhắc lịch thủ công. |

**Vote: 1/7**

---

## (6) Đăng

**Bài toán:** Tester viết test case — Mỗi tính năng thì cần phải viết nhiều test case, tuy nhiên nội dung test có thể giống nhau chỉ khác một chút → AI gen test case, reuse

### Challenge & Trả lời

| Câu hỏi | Trả lời |
|:---|:---|
| AI tạo ra các test case vô nghĩa (chỉ đổi input) thì sao? | Yêu cầu AI tạo các test case cho các trường dữ liệu đại diện hoặc dữ liệu biên |
| Nếu logic tính năng thay đổi thì AI có gen lại toàn bộ test case của tính năng đó không? | Hướng dẫn AI viết theo hướng Data-Driven Testing |

### Cards bị loại

| Card bị loại | Lý do |
|:---|:---|
| Khi team có người mới thì cần training từ đầu về luồng hoạt động, code base, tài liệu... | Có nhiều AI hỗ trợ như NotebookLM giúp đọc tài liệu, Code Assist giúp giải thích code… |
| Tìm hiểu công nghệ mới để áp dụng trong thực tế | Ưu tiên chọn công nghệ, framework ổn định, cộng đồng support lớn |

**Vote: 1/7**

---

## (7) Ngọc

### Phase 3 — PITCH-CHALLENGE-VOTE

**Card #1 - Xử lý khiếu nại khách hàng (Customer Grievance Resolution)**

### Challenge & Trả lời

| Câu challenge | Câu trả lời |
|:---|:---|
| Rule/script đủ chưa? Có thật sự cần AI không? | Rule không thể bao quát văn bản tự do. Lịch sử trên CRM là text do nhân viên tự gõ, nhiều tiếng lóng/viết tắt. Việc xử lý hiện tại bắt buộc phải chuyển qua lại nhiều bộ phận (Sales, Collection) để lấy thông tin thủ công. Rất dễ bỏ sót thông tin. Chỉ có LLM Feature mới đọc hiểu và xâu chuỗi được logic ai đúng ai sai. |
| Ngoài bạn, ai đau nữa? Quy mô bao nhiêu người? | Toàn bộ phòng CSKH chuyên giải quyết khiếu nại Escalation (khoảng 20 chuyên viên) đều mắc kẹt ở khâu này. Trung bình mỗi ngày team nhận ~200 ticket khó. Khách hàng đợi lâu 4-6 tiếng nên thường nóng giận, dẫn đến khiếu nại leo thang, nhân viên áp lực cục bộ. |
| Metric đo được không? Có số cụ thể chưa? | Đo được rõ ràng. Trung bình mỗi khiếu nại mất 4–6 tiếng (có trường hợp vài ngày). AI giúp rút ngắn tổng thời gian xử lý xuống còn ~1 tiếng/ticket. Thời gian tiết kiệm được sẽ dùng để tập trung chăm sóc khách VIP và phân tích nguyên nhân gốc rễ (Root cause) để cải thiện sản phẩm, tăng hài lòng dài hạn thay vì chỉ đi "dập lửa". |

**Vote: 5/7**

### Lý do Kill Cards

| Card bị loại | Lý do |
|:---|:---|
| Chấm điểm QA | Bài toán hay và impact rõ (metric tốt), nhưng phụ thuộc cực kỳ lớn vào chất lượng Speech-to-Text tiếng Việt vùng miền (đây là Risk về Core Tech, khó demo proof-of-concept thành công). |
| Collections Report | Giải quyết bài toán này bản chất chỉ cần Rules (RPA/ETL Scripts), không có nhu cầu "Semantic/Context" rõ rệt để cần tới sức mạnh của GenAI. "Rule đủ rồi". |

---

## Phase 3 — PITCH-CHALLENGE-VOTE (Anh)

**Anh pitch đề tài cho nhóm (2 min):**

> "Hiện tại mỗi khi cần di chuyển nhanh và tiết kiệm, tôi phải mở cả 3 app Grab, Xanh SM, Be để so sánh giá và thời gian chờ. Bước này tốn ít nhất 5 phút và cực kỳ gây ức chế khi đang vội. Nếu có AI tự động thu thập và đề xuất phương tiện tối ưu ngay lập tức, chúng ta sẽ tiết kiệm được rất nhiều thời gian và tiền bạc."

- **Bước 1-3**: Manual checking từng app, không real-time.
- **Bước 4**: Manual comparison, dễ miss optimal choice.
- **Rủi ro**: Chọn sai dẫn đến chậm trễ hoặc tốn kém.

### 4.2 — Problem Statement (6-field)

- **Actor**: Product Manager tại công ty logistics, chịu trách nhiệm optimize transportation cho users
- **Current Workflow**: Mỗi lần đi: check Grab → check Xanh → check Be → compare → choose. 5 bước, 16 phút, thủ công
- **Bottleneck**: Bước check và compare mất 13 phút (81% thời gian) vì phải manual từng app, không có aggregation
- **Impact**: 16 phút/lần × 2-3 lần/ngày = ~1 giờ/ngày cho 1 user. 1000 users → ~1000 giờ/ngày. 70% users chọn không optimal
- **Success Metric**: Giảm thời gian chọn từ 16 phút xuống dưới 2 phút (88% reduction). Tỉ lệ chọn optimal từ 30% lên 90%
- **Operational Boundary**: AI được phép thu thập data từ apps và suggest options. AI không được tự book rides, user phải confirm

### 4.3 — Research

**Existing Solutions**

| Giải pháp | Điểm mạnh | Điểm yếu |
|:---|:---|:---|
| Grab/Xanh/Be apps | Individual apps | No cross-platform comparison |
| Google Maps | Route planning | Không price comparison |
| Rome2Rio | Multi-transport comparison | Focus international |

**Case Studies**

- **Uber's surge pricing**: ML predicts prices, nhưng không cross-app
- **Citymapper**: Multi-modal transport, nhưng manual price check
- **Internal logistics**: Companies build internal tools cho fleet optimization

**Quick Poll Results**

- User A: Check all apps manually, takes 10-15 min
- User B: Usually use Grab, sometimes regret
- User C: Ask friends for recommendations
- User D: Use whatever is cheapest, ignore time

*Insights*: Universal pain, high demand for AI solution

---

# 02 — Deep Dive Report

**Bài toán được chọn:** Đề xuất phương tiện di chuyển khả dụng + nhanh + rẻ dựa trên thu thập dữ liệu real-time từ Grab, Xanh SM, Be

---

## 4.1 — Workflow Mapping (Current State)

### Actor chính

- **Người dùng A:** Đi lại hàng ngày (sinh viên, nhân viên văn phòng) — ưu tiên rẻ + quen tuyến
- **Người dùng B:** Đi lại thỉnh thoảng, không có xe cá nhân — ưu tiên nhanh + khả dụng

### Workflow hiện tại (As-Is)

```
TRIGGER: Người dùng cần di chuyển từ A → B
         │
         ▼
Bước 1: Mở app thủ công (3 app riêng lẻ)
         Mở lần lượt từng app (Grab → Be → Xanh)
         Áp mã giảm giá (nếu có)          ⏱ 1–2 min / 3 app
         │
         ▼
Bước 2: Nhập điểm đi–đến trên từng app
         Nhập điểm đi / điểm đến 3 lần
         Áp mã giảm giá (nếu có)          ⏱ 1–2 min (lặp lại)
         │
         ▼
Bước 3: So sánh thủ công giá + ETA + loại xe
         Xem giá, loại xe, ETA — mỗi app 1 format khác
         ⏱ 2–3 min (cộng dồn) ★ BOTTLENECK CHÍNH
         │
         ▼
Bước 4: Đặt — chờ xác nhận (có thể bị hủy)
         Không rõ tài xế có nhận không, giờ cao điểm
         có thể hủy / không khớp          ⏱ 1–5 min
         │
         ▼
Bước 5: Di chuyển / quay lại so sánh
         Nếu bị hủy: quay lại bước 1
         Nếu ok: hoàn thành
```

**Thời gian tổng (trước khi lên xe):** 5–12 phút  
**Tần suất:** 1–4 lần/ngày với người dùng thường xuyên

### Bottleneck xác định

| Bước | Vấn đề | Thời gian mất |
|:---|:---|:---|
| Bước 2 | Nhập lại điểm đi–đến 3 lần | ~3 min |
| Bước 3 | So sánh thủ công, format khác nhau, không có baseline chung | ~3 min |
| Bước 4 | Không biết trước khả năng có tài xế hay không | ~2 min |

---

## 4.2 — Problem Statement (6-field PS)

| Field | Nội dung |
|:---|:---|
| **Actor** | Người dùng ride-hailing tại Việt Nam (cả người đi hàng ngày lẫn thỉnh thoảng), không có xe cá nhân hoặc chủ động chọn không dùng xe |
| **Situation** | Khi cần di chuyển từ điểm A đến điểm B — đặc biệt giờ cao điểm, thời tiết xấu, hoặc khi ngân sách bị giới hạn |
| **Job-to-be-done** | Chọn được phương tiện phù hợp nhất (theo bộ ưu tiên cá nhân: rẻ / nhanh / chắc có xe) mà không phải tự mở và so sánh nhiều app |
| **Pain** | Phải mở 3 app riêng lẻ, nhập lại thông tin nhiều lần, so sánh thủ công các format khác nhau, và vẫn không chắc có tài xế nhận không — tốn 5–12 phút trước khi lên xe |
| **Metric thành công** | Thời gian từ "có nhu cầu" đến "đặt xong" giảm từ 5–12 phút xuống dưới 90 giây; tỉ lệ đặt thành công lần đầu tăng từ ~70% lên trên 90% |
| **Boundary** | Chỉ xử lý bước so sánh + đề xuất — **không** tự động đặt xe thay người dùng; người dùng vẫn bấm xác nhận cuối |

### Primary metrics

| Metric | Baseline hiện tại | Target |
|:---|:---|:---|
| Thời gian từ mở tool → đặt xong | 5–12 phút | < 90 giây |
| Số bước người dùng phải thao tác | ~15 bước (3 app × 5 bước) | ≤ 3 bước |
| Tỉ lệ đặt thành công lần đầu | ~70% (ước tính) | > 90% |
| Tỉ lệ hài lòng với lựa chọn được đề xuất | Không đo được | > 80% thumbs up |

### Guardrail metrics (không được phá vỡ)

- Độ trễ fetch data từ 3 app ≤ 3 giây (không làm tổng thời gian tệ hơn baseline)
- Không lưu thông tin tài khoản / thanh toán của người dùng
- Khi 1 app trả về lỗi → hiển thị rõ, không silently drop option

### Boundary rõ ràng

✅ **Trong scope:**
- Fetch giá + ETA + loại xe từ 3 app theo thời gian thực
- Xếp hạng / đề xuất theo bộ ưu tiên người dùng chọn
- Cảnh báo khi khả dụng thấp (surge pricing, ít tài xế)
- Giải thích lý do đề xuất ("rẻ hơn Be 12k, ETA gần bằng")

❌ **Ngoài scope:**
- Tự động đặt xe (người dùng vẫn xác nhận)
- Tích hợp thanh toán
- Theo dõi chuyến đi sau khi đặt
- So sánh với xe buýt / metro (phase 2)

---

## 4.3 — Research

### Existing solutions

| Giải pháp | Điểm mạnh | Điểm yếu |
|:---|:---|:---|
| **Mogi / Gojek (Indonesia)** | Super-app tích hợp nhiều dịch vụ | Không có tại VN, không so sánh cross-app |
| **Google Maps** | Gợi ý phương tiện công cộng + đi bộ | Không có giá ride-hailing real-time |
| **Grab "So sánh dịch vụ"** | So sánh trong nội bộ Grab (GrabBike vs GrabCar) | Chỉ trong 1 app, không cross-platform |
| **Extension / script tự làm** | Một số dev đã làm unofficial scraper | Không ổn định, dễ bị block, không có UX |

**Kết luận:** Thị trường VN chưa có giải pháp so sánh cross-app ride-hailing một cách chính thức và có UX tốt.

### Case study tham khảo

- **Skyscanner / Google Flights:** So sánh giá vé nhiều hãng hàng không → mô hình aggregate + rank tương tự bài toán này
- **Kayak cho xe thuê:** Rank theo giá + availability + reviews → AI fit: rule-based ranking + LLM để giải thích recommendation

### Quick poll (quan sát từ cộng đồng)

- Group Facebook "Hội ghét kẹt xe Hà Nội / HCM": người dùng thường xuyên hỏi nhau "Grab hay Be rẻ hơn giờ này?"
- Reddit r/VietNam: một số thread so sánh app, phần lớn dựa trên kinh nghiệm cá nhân, không có data real-time
- **Bài học:** Nhu cầu so sánh có thật, đang được giải quyết bằng "hỏi cộng đồng" — tức là chưa có tool tốt

### Buy / Boost / Build?

- **Buy:** Không có sản phẩm nào đang bán đúng use case này tại VN
- **Boost:** Có thể dùng API của từng app nếu được cấp quyền (Grab có Partner API)
- **Build:** Cần xây aggregation layer + ranking logic + UI — feasible ở mức MVP

---

## 4.4 — Future-State Flow + AI Fit

### AI Fit Check

```
Complexity của task:    THẤP  ─●──── CAO
                                 ↑
                         Ranking + explain

Ambiguity của output:   THẤP  ────●────── CAO
                               ↑
                    Output khá có cấu trúc
                    (giá, ETA, loại xe)
                    nhưng cần diễn đạt tự nhiên
```

→ **Vùng:** LLM Feature (ranking + natural language explanation)  
→ Phần fetch + aggregate: Rule / API call đủ  
→ Phần rank + giải thích "tại sao chọn cái này": LLM phù hợp

### AI Suitability Check

| Tiêu chí | Đánh giá |
|:---|:---|
| Cần xử lý ngôn ngữ tự nhiên? | ✓ (giải thích recommendation) |
| Output đa dạng tốt hơn cố định? | △ (output có cấu trúc, nhưng ngữ cảnh thay đổi theo user) |
| Rule-based có đủ không? | △ (rule đủ để rank, nhưng không đủ để giải thích linh hoạt) |
| Sai thì hậu quả nghiêm trọng? | ✗ (người dùng vẫn xác nhận trước khi đặt — failure cost thấp) |
| Cần học từ hành vi người dùng? | ✓ (ưu tiên rẻ/nhanh/khả dụng thay đổi theo người và thời điểm) |

### Vì sao không phải Agent

1. Workflow tuyến tính: fetch → rank → hiển thị → người dùng chọn
2. Không cần AI tự quyết định multi-step động
3. Phần cần AI chỉ là bước rank + explain — không phải toàn bộ flow

### Future-State Flow (To-Be)

```
┌──────────────────┐
│ Người dùng nhập  │   Chỉ nhập 1 lần: điểm đi, điểm đến
│ điểm đi / đến   │   (+ tuỳ chọn: ưu tiên rẻ / nhanh / chắc có xe)
└──────────────────┘
         │
         ▼
┌──────────────────┐
│ 🔵 Auto-fetch    │   Gọi API Grab + Be + Xanh SM đồng thời
│ data 3 app       │   ⏱ mục tiêu: ≤ 3 giây
│ (parallel call)  │
└──────────────────┘
         │
         ▼
┌──────────────────┐
│ 🔵 LLM rank +    │   Xếp hạng theo ưu tiên người dùng
│ explain          │   Sinh câu giải thích tự nhiên:
│                  │   "Be rẻ hơn 15k, ETA chênh 2 phút"
└──────────────────┘
         │
         ▼
┌──────────────────┐
│ 🟢 Người dùng    │   Xem top 1–3 đề xuất
│ review + chọn   │   Bấm "Mở app" để đặt
│ 🔴 Boundary:     │
│ người dùng xác   │
│ nhận cuối        │
└──────────────────┘
```

➡️ **Fallback:** Nếu 1 app lỗi → hiển thị 2 app còn lại, ghi rõ thiếu dữ liệu từ app nào  
➡️ **Fallback:** Nếu LLM chậm → hiển thị bảng rank đơn giản không có explanation

### Underspecification Check

| Điều chưa rõ | Hậu quả nếu sai | Cách validate |
|:---|:---|:---|
| Grab / Be có cho phép fetch giá real-time không? | Không build được nếu không có API hợp lệ | Check Grab Partner API, Be API docs |
| "Khả dụng" đo bằng gì? (ETA? Số tài xế gần?) | Rank sai nếu dùng metric không đúng | Pilot: dùng ETA làm proxy trước |
| Người dùng có thật sự đổi app nếu rẻ hơn 5k không? | Build tool mà không ai dùng | User interview 5–10 người |
| Surge pricing có expose qua API không? | Thiếu thông tin quan trọng nhất lúc cao điểm | Test thực tế giờ cao điểm |

---

## 4.5 — AI Readiness Checklist

| # | Câu hỏi | Kết quả | Ghi chú |
|:---|:---|:---|:---|
| 1 | Có data/input đủ chất lượng? | △ | Phụ thuộc vào API access — cần xác nhận |
| 2 | Có metric rõ? | ✓ | < 90 giây, > 90% đặt thành công lần đầu |
| 3 | Sai thì hậu quả chấp nhận được? | ✓ | Người dùng vẫn xác nhận trước khi đặt |
| 4 | User sẵn sàng dùng AI? | ✓ | Nhu cầu có thật, đang giải quyết bằng "hỏi cộng đồng" |
| 5 | Có resource để build + maintain? | △ | Cần dev có thể gọi API + basic LLM integration |

---

# Phase 5 — EVALUATE

| Câu hỏi | Kết Quả | Ghi chú |
|:---|:---|:---|
| Có data/input đủ chất lượng? | Yes | Grab, Be, XanhSM |
| Có metric rõ? | Yes | Giá tiền là metric rõ ràng nhất |
| Sai thì hậu quả có chấp nhận được? | Yes | Chi phí chênh lệch sẽ không quá cao |
| Có resource để maintain? | No | Cần Dev để build |

**Rủi ro:**
- Thay đổi API làm hỏng hệ thống
- Các khuyến nghị sai lệch làm tổn hại lòng tin
- Lo ngại về quyền riêng tư với việc thu thập dữ liệu

---

## Quyết định: GO (với điều kiện)

### Justify

- 3/5 điều kiện rõ ràng đã đủ
- 2 điều kiện còn lại (API access + dev resource) là **rủi ro kỹ thuật**, không phải problem sai
- Nhu cầu được validate qua hành vi thật (người dùng đang tự so sánh thủ công hàng ngày)
- Failure cost thấp: người dùng vẫn xác nhận → AI sai thì người dùng chỉnh được

### Điều kiện cần validate trước khi build

1. **API feasibility:** Xác nhận Grab Partner API + Be API cho phép fetch giá real-time
2. **User threshold:** Interview nhanh — người dùng có đổi app nếu rẻ hơn bao nhiêu?
3. **Surge pricing signal:** Test thực tế giờ cao điểm xem data có expose không

### Nếu API không available

→ **Fallback plan:** Dùng web scraping có kiểm soát (rủi ro ToS) hoặc hạ scope xuống chỉ so sánh 2 app có API mở  
→ Hoặc pivot sang: tool giúp người dùng **học pattern** ("Be thường rẻ hơn Grab ~15% vào giờ thấp điểm") thay vì real-time fetch

### Optimization check

**Lợi ích rõ:**
- Tiết kiệm 5–10 phút/lần đặt xe, 1–4 lần/ngày → ~10–40 phút/ngày với người dùng thường xuyên
- Giảm cognitive load khi đang vội hoặc dưới mưa

**Rủi ro nếu optimize sai:**
- LLM giải thích sai lý do đề xuất (hallucinate giá) → người dùng mất tin tưởng
- Fetch data bị delay → đề xuất dựa trên giá cũ, thực tế khác
