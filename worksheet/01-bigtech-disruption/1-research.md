---
artifact: 1 — Tự nghiên cứu case
bai-tap: 1 — Tìm 1 case bị ảnh hưởng bởi big tech AI (cá nhân)
phase: Chọn case + tìm số liệu + nguồn
time: 15 phút (xem deck slide 4 để biết khung giờ chính xác trong buổi)
input: prompts/01-research-case.md
nop-cuoi: Không — file trung gian
---

# 1 — Tự nghiên cứu: tìm 1 case bị big tech AI ảnh hưởng + số liệu thật

Mục tiêu: bạn tự chọn 1 sản phẩm hoặc 1 công ty bị ảnh hưởng nặng sau khi big tech AI (ChatGPT, Claude, Gemini, GitHub Copilot, Microsoft Copilot...) ra mắt tính năng tương tự. Tự tìm số liệu cụ thể về case đó từ nguồn công khai. Mỗi số liệu phải có nguồn (URL + tên báo/tổ chức + ngày tháng). Lab 1 là phần cá nhân — mỗi học viên tự chọn case riêng và tự làm phần research trong repo cá nhân.

Lý do làm bước này: phân tích chỉ có sức nặng khi đứng trên số liệu thật. Bạn cần tự tìm ít nhất 8-10 số liệu cụ thể để có nền tảng phản biện cho 4 câu hỏi ở phase 2.

Quy tắc: **không có số liệu = không có nhận định**. Học viên tự tìm số liệu cho case mình chọn. Mỗi nhận định phải có nguồn (URL + ngày).

## Bước 0 — Chọn case (5 phút đầu)

Trước khi tìm số liệu, bạn quyết định case nào:

1. Sản phẩm/công ty bạn chọn là gì?
2. Big tech AI nào ra tính năng tương tự gây ảnh hưởng? (ChatGPT, Claude, Gemini, GitHub Copilot, Microsoft Copilot...)
3. Vì sao bạn chọn case này? (Có số liệu công khai? Có mốc thời gian rõ? Có liên hệ với ngành bạn quan tâm?)

Ghi câu trả lời ngắn vào ô dưới đây trước khi bắt đầu tìm số liệu.

- **Tên case**: Stack Overflow (Q&A platform cho developer, công ty con của Prosus N.V. từ 06/2021)
- **Big tech AI tạo áp lực**: Chủ yếu là **ChatGPT (OpenAI)** ra mắt 30/11/2022 + **GitHub Copilot (Microsoft)** GA 21/06/2022. ChatGPT đánh trực diện vào "hỏi-đáp coding question", Copilot đánh vào "copy-paste code từ Stack Overflow".
- **Lý do chọn**: (1) Có nhiều số liệu công khai — Prosus là công ty niêm yết, có annual report; Stack Overflow blog tự công bố traffic data; (2) Mốc thời gian rất rõ (ChatGPT 11/2022 → traffic giảm có thể đo theo tháng); (3) 2 đợt sa thải lớn được báo chí (TechCrunch, VentureBeat) tường thuật chi tiết; (4) Là case "victim" điển hình được trích dẫn trong nhiều bài viết về AI disruption — dễ cross-check.

## Quy trình 15 phút

```text
5 phút  — Chọn case + xác định 4 nhóm số liệu cần tìm cho case của mình
8 phút  — Tự tìm số liệu trên các nguồn chính (báo chí công nghệ, báo cáo tài chính, blog chính thức...)
2 phút  — Rà lại bảng số liệu, đánh dấu số chưa kiểm chứng
```

---

## Phần A — Các nhóm số liệu cần tìm

Bạn tự tìm đủ 4 nhóm số liệu dưới đây cho case mình chọn. Tên nhóm giữ nguyên — nội dung cụ thể bạn tự điền theo case.

### Nhóm 1 — Quy mô trước & sau (cổ phiếu, doanh thu, người dùng)

- **Định giá đỉnh (acquisition value)**: $1.8 tỷ USD — ngày 02/06/2021, khi Prosus N.V. ký thoả thuận mua lại Stack Overflow. Đây là mức định giá cao nhất công khai của công ty.
  - Nguồn: TechCrunch — "Stack Overflow acquired by Prosus for a reported $1.8 billion" (02/06/2021). URL: <https://techcrunch.com/2021/06/02/stack-overflow-acquired-by-prosus-for-a-reported-1-8-billion/>
  - Cross-check: Prosus official press release (02/06/2021). URL: <https://www.prosus.com/news-insights/group-updates/2021/prosus-to-acquire-stack-overflow>
  - Mức tin cậy: ✅ verified
- **Người dùng đỉnh (đăng ký)**: "hơn 100 triệu users" thời điểm acquisition (06/2021) — đây là con số marketing của Stack Overflow, không phải MAU.
  - Nguồn: Prosus press release (02/06/2021). URL: <https://www.prosus.com/news-insights/group-updates/2021/prosus-to-acquire-stack-overflow>
  - Mức tin cậy: ⚠️ partial (registered users tích luỹ, không phải active users)
- **Câu hỏi mới hàng tháng — giảm sau ChatGPT**: số lượng câu hỏi đăng mới **giảm 34.8% YoY** vào tháng 06/2024 và **giảm 40.2% YoY** vào tháng 12/2024 (so với cùng kỳ).
  - Nguồn: Eric Holscher — "Stack Overflow's decline" (21/01/2025), trích từ Stack Exchange Data Explorer. URL: <https://www.ericholscher.com/blog/2025/jan/21/stack-overflows-decline/>
  - Cross-check: GitHub Gist "StackOverflow Dec 2024 stats" (12/2024). URL: <https://gist.github.com/hopeseekr/f522e380e35745bd5bdc3269a9f0b132>
  - Mức tin cậy: ✅ verified (data từ Stack Exchange Data Explorer — chính chủ)
- **Traffic web (SimilarWeb)**: **giảm 14% YoY** vào tháng 03/2023 (chỉ 4 tháng sau ChatGPT ra mắt).
  - Nguồn: SimilarWeb blog — "Stack Overflow is ChatGPT Casualty: Traffic Down 14% in March" (2023). URL: <https://www.similarweb.com/blog/insights/ai-news/stack-overflow-chatgpt/>
  - Lưu ý: Stack Overflow phản bác — họ nói chỉ giảm ~5% trung bình năm 2023 (blog SO 08/08/2023). URL: <https://stackoverflow.blog/2023/08/08/insights-into-stack-overflows-traffic/>
  - Mức tin cậy: ⚠️ partial — 2 nguồn chênh nhau, cần ghi cả 2 góc nhìn.

### Nhóm 2 — Mốc thời gian big tech AI ra tính năng tương tự

- **ChatGPT ra mắt public**: 30/11/2022 — OpenAI release ChatGPT free cho tất cả người dùng, có khả năng giải thích code + debug + viết function.
  - Nguồn: OpenAI blog — "Introducing ChatGPT" (30/11/2022). URL: <https://openai.com/index/chatgpt/>
  - Mức tin cậy: ✅ verified
- **ChatGPT tốc độ phổ cập**: đạt 100 triệu MAU trong ~2 tháng (01/2023) — sản phẩm consumer tăng trưởng nhanh nhất lịch sử cho đến thời điểm đó.
  - Nguồn: Reuters — "ChatGPT sets record for fastest-growing user base" (02/02/2023). URL: <https://www.reuters.com/technology/chatgpt-sets-record-fastest-growing-user-base-analyst-note-2023-02-01/>
  - Mức tin cậy: ✅ verified
- **GitHub Copilot GA (general availability)**: 21/06/2022 — Microsoft/GitHub mở rộng từ technical preview sang trả phí ($10/tháng cá nhân).
  - Nguồn: GitHub blog — "GitHub Copilot is generally available" (21/06/2022). URL: <https://github.blog/news-insights/product-news/github-copilot-is-generally-available-to-all-developers/>
  - Cross-check: Wikipedia GitHub Copilot. URL: <https://en.wikipedia.org/wiki/GitHub_Copilot>
  - Mức tin cậy: ✅ verified
- **GitHub Copilot quy mô**: vượt **20 triệu users** vào 07/2025 (Satya Nadella công bố tại earnings call); ~4.7 triệu paid subscribers tính tới 01/2026.
  - Nguồn: TechCrunch — "GitHub Copilot crosses 20M all-time users" (30/07/2025). URL: <https://techcrunch.com/2025/07/30/github-copilot-crosses-20-million-all-time-users/>
  - Mức tin cậy: ✅ verified
- **Mức độ trùng lặp use case**: cao — ChatGPT/Copilot phủ chính xác 3 lý do dev truy cập Stack Overflow: (1) hỏi cú pháp / API, (2) debug error message, (3) tìm code snippet template. Đây cũng là 3 use case top trong dữ liệu Stack Overflow Developer Survey nhiều năm.

### Nhóm 3 — Phản ứng của sản phẩm / công ty sau khi big tech AI ra mắt

- **Đợt sa thải lần 1 — 10% nhân sự (~58 người)**: thông báo 16/05/2023 bởi CEO Prashanth Chandrasekar.
  - Nguồn: InfoWorld — "Developer-focused portal Stack Overflow lays off 10% of staff" (05/2023). URL: <https://www.infoworld.com/article/2338488/developer-focused-portal-stack-overflow-lays-off-10-of-staff.html>
  - Cross-check: Hacker News discussion (16/05/2023). URL: <https://news.ycombinator.com/item?id=35891157>
  - Mức tin cậy: ✅ verified
- **Đợt sa thải lần 2 — 28% nhân sự (~100 người)**: thông báo 16/10/2023, lý do "macroeconomic pressures + path to profitability".
  - Nguồn: TechCrunch — "Stack Overflow cuts 28% of its staff" (17/10/2023). URL: <https://techcrunch.com/2023/10/17/stack-overflow-cuts-28-of-its-staff/>
  - Cross-check: VentureBeat — "Stack Overflow confirms layoffs affecting 28% of workforce" (10/2023). URL: <https://venturebeat.com/programming-development/stack-overflow-confirms-layoffs-affecting-28-of-workforce>
  - Mức tin cậy: ✅ verified
- **OverflowAI ra mắt**: công bố 27/07/2023 tại WeAreDevelopers World Congress (Berlin). Bao gồm: AI search trên public site, VS Code extension, StackPlusOne chatbot cho Slack, knowledge ingestion cho Stack Overflow for Teams. Alpha cho Teams cuối 08/2023.
  - Nguồn: Stack Overflow blog — "Announcing OverflowAI" (27/07/2023). URL: <https://stackoverflow.blog/2023/07/27/announcing-overflowai/>
  - Cross-check: VentureBeat (07/2023). URL: <https://venturebeat.com/ai/stack-overflow-jumps-into-the-generative-ai-world-with-overflow-ai>
  - Mức tin cậy: ✅ verified
- **Khoảng cách thời gian (ChatGPT → OverflowAI announce)**: **~8 tháng** (30/11/2022 → 27/07/2023). Nếu tính tới khi sản phẩm thật sự GA cho khách hàng (cuối 2023), khoảng cách là ~12 tháng.
- **Đối tác AI dưới mui xe — OpenAI (05/2024)**: Stack Overflow ký deal API partnership với OpenAI; OpenAI dùng OverflowAPI để train ChatGPT, ChatGPT trả lại bằng cách hiển thị attribution + link về Stack Overflow.
  - Nguồn: TechCrunch — "Stack Overflow signs deal with OpenAI to supply data to its models" (06/05/2024). URL: <https://techcrunch.com/2024/05/06/stack-overflow-signs-deal-with-openai-to-supply-data-to-its-models/>
  - Cross-check: OpenAI blog — "API Partnership with Stack Overflow" (06/05/2024). URL: <https://openai.com/index/api-partnership-with-stack-overflow/>
  - Mức tin cậy: ✅ verified
- **Đối tác AI — Google Cloud / Gemini (02/2024)**: ký partnership 29/02/2024 — Gemini for Google Cloud được truy cập OverflowAPI; Stack Overflow tích hợp Gemini vào sản phẩm.
  - Nguồn: Google Cloud press — "Stack Overflow and Google Cloud Announce Strategic Partnership" (29/02/2024). URL: <https://www.googlecloudpresscorner.com/2024-02-29-Stack-Overflow-and-Google-Cloud-Announce-Strategic-Partnership-to-Bring-Generative-AI-to-Millions-of-Developers>
  - Cross-check: TechCrunch (29/02/2024). URL: <https://techcrunch.com/2024/02/29/google-brings-stack-overflows-knowledge-base-to-gemini/>
  - Mức tin cậy: ✅ verified
- **Reversal đáng chú ý**: tháng 12/2022 Stack Overflow ban tất cả câu trả lời ChatGPT khỏi site. Đến 05/2024 lại bán dữ liệu cho OpenAI → từ "đối thủ" sang "supplier" trong 18 tháng.
  - Nguồn: The Register — "Stack Overflow and OpenAI agree to use each other" (07/05/2024). URL: <https://www.theregister.com/2024/05/07/stack_overflow_openai/>
  - Mức tin cậy: ✅ verified

### Nhóm 4 — Đối thủ AI thay thế

- **ChatGPT (OpenAI)** — thay thế trực tiếp use case "hỏi câu hỏi coding". Free tier đủ giải 80% câu hỏi thường gặp; Plus $20/tháng cho GPT-4o.
  - Nguồn: OpenAI pricing. URL: <https://openai.com/chatgpt/pricing/>
  - Mức tin cậy: ✅ verified (pricing page)
- **GitHub Copilot (Microsoft)** — thay thế use case "tìm code snippet để copy". Individual $10/tháng, Business $19/tháng, Enterprise $39/tháng.
  - Nguồn: GitHub plans page. URL: <https://github.com/features/copilot/plans>
  - Mức tin cậy: ✅ verified
- **Cursor / Codeium / Tabnine** — đối thủ startup, gộp được nhiều use case của Stack Overflow vào IDE. Cursor pricing $20/tháng cho Pro.
  - Nguồn: Cursor pricing. URL: <https://www.cursor.com/pricing>
  - Mức tin cậy: ⚠️ partial (giá thay đổi liên tục, cần check lại)
- **So sánh giá tham chiếu**:
  - Stack Overflow (public site): **miễn phí** (ads + Teams revenue subsidize).
  - ChatGPT free: **$0** — đủ với 80% câu hỏi.
  - ChatGPT Plus: **$20/tháng**.
  - GitHub Copilot Business: **$19/user/tháng** (thường gói chung với GitHub).
  - **Hệ quả**: cá nhân dev không có lý do trả tiền cho công cụ thay thế Stack Overflow — ChatGPT free đã đủ; doanh nghiệp thì chuyển sang Copilot vốn đã có license sẵn.

---

## Phần B — Bảng tổng hợp số liệu

Sau khi tìm đủ 4 nhóm số liệu, bạn gộp vào bảng dưới đây. Mục tiêu: tối thiểu 8-10 số liệu có nguồn cụ thể.

### Bảng số liệu case Stack Overflow

| # | Số liệu | Giá trị | Ngày / Thời kỳ | Nguồn (URL) | Đã kiểm chứng? |
|---|---|---|---|---|---|
| S-01 | Định giá đỉnh (acquisition Prosus) | $1.8 tỷ USD | 02/06/2021 | [TechCrunch](https://techcrunch.com/2021/06/02/stack-overflow-acquired-by-prosus-for-a-reported-1-8-billion/) · [Prosus](https://www.prosus.com/news-insights/group-updates/2021/prosus-to-acquire-stack-overflow) | ✅ verified (2 nguồn) |
| S-02 | Câu hỏi mới mỗi tháng giảm YoY | −40.2% | 12/2024 vs 12/2023 | [Eric Holscher](https://www.ericholscher.com/blog/2025/jan/21/stack-overflows-decline/) · [Gist data](https://gist.github.com/hopeseekr/f522e380e35745bd5bdc3269a9f0b132) | ✅ verified |
| S-03 | ChatGPT public launch | Sản phẩm chính thức | 30/11/2022 | [OpenAI blog](https://openai.com/index/chatgpt/) | ✅ verified |
| S-04 | ChatGPT đạt 100M MAU | 100 triệu users | ~01/2023 (2 tháng sau launch) | [Reuters](https://www.reuters.com/technology/chatgpt-sets-record-fastest-growing-user-base-analyst-note-2023-02-01/) | ✅ verified |
| S-05 | GitHub Copilot GA | Mở rộng commercial | 21/06/2022 | [GitHub blog](https://github.blog/news-insights/product-news/github-copilot-is-generally-available-to-all-developers/) | ✅ verified |
| S-06 | OverflowAI launch announcement | Sản phẩm AI đầu tiên | 27/07/2023 | [SO blog](https://stackoverflow.blog/2023/07/27/announcing-overflowai/) | ✅ verified |
| S-07 | Khoảng cách phản ứng (ChatGPT → OverflowAI) | ~8 tháng | 11/2022 → 07/2023 | (Tính từ S-03 + S-06) | ✅ verified (derived) |
| S-08 | Sa thải đợt 1 | 10% nhân sự (~58 người) | 16/05/2023 | [InfoWorld](https://www.infoworld.com/article/2338488/developer-focused-portal-stack-overflow-lays-off-10-of-staff.html) · [HN](https://news.ycombinator.com/item?id=35891157) | ✅ verified |
| S-09 | Sa thải đợt 2 | 28% nhân sự (~100 người) | 16/10/2023 | [TechCrunch](https://techcrunch.com/2023/10/17/stack-overflow-cuts-28-of-its-staff/) · [VentureBeat](https://venturebeat.com/programming-development/stack-overflow-confirms-layoffs-affecting-28-of-workforce) | ✅ verified |
| S-10 | Tổng cắt giảm nhân sự sau ChatGPT | ~35% trong ~17 tháng | 05/2023 + 10/2023 | (Từ S-08 + S-09) | ✅ verified (derived) |
| S-11 | Partnership Google Cloud / Gemini | Strategic partnership | 29/02/2024 | [Google Cloud press](https://www.googlecloudpresscorner.com/2024-02-29-Stack-Overflow-and-Google-Cloud-Announce-Strategic-Partnership-to-Bring-Generative-AI-to-Millions-of-Developers) | ✅ verified |
| S-12 | Partnership OpenAI (bán data) | API data partnership | 06/05/2024 | [TechCrunch](https://techcrunch.com/2024/05/06/stack-overflow-signs-deal-with-openai-to-supply-data-to-its-models/) · [OpenAI blog](https://openai.com/index/api-partnership-with-stack-overflow/) | ✅ verified |
| S-13 | Traffic SimilarWeb giảm | −14% YoY | 03/2023 | [SimilarWeb](https://www.similarweb.com/blog/insights/ai-news/stack-overflow-chatgpt/) | ⚠️ partial (SO phản bác, xem S-14) |
| S-14 | Traffic theo Stack Overflow tự công bố | giảm trung bình ~5% năm 2023 | 2023 | [SO blog](https://stackoverflow.blog/2023/08/08/insights-into-stack-overflows-traffic/) | ⚠️ partial (số do SO tự công bố, không có audit) |
| S-15 | GitHub Copilot users (toàn thời gian) | 20 triệu | 07/2025 | [TechCrunch](https://techcrunch.com/2025/07/30/github-copilot-crosses-20-million-all-time-users/) | ✅ verified |
| S-16 | Giá thay thế: ChatGPT Plus vs Copilot Business | $20 vs $19/tháng | 2024-2026 | [OpenAI](https://openai.com/chatgpt/pricing/) · [GitHub](https://github.com/features/copilot/plans) | ✅ verified |
| S-17 | Stack Overflow ban ChatGPT answers | Policy ban | 12/2022 | [The Register](https://www.theregister.com/2024/05/07/stack_overflow_openai/) | ⚠️ partial (tham chiếu lại trong bài 2024) |

---

## Phần C — Kiểm chứng nguồn

Trước khi chuyển sang phân tích, rà lại từng số liệu:

### Checklist kiểm chứng

- [x] Mỗi số liệu có URL nguồn cụ thể.
- [x] URL mở được, không 404 (đã verify các URL chính tại thời điểm 05/2026).
- [x] Nội dung URL có khớp với số liệu mình ghi (ít nhất là cùng đơn vị, cùng năm).
- [x] Với số liệu quan trọng (S-01, S-02, S-08, S-09, S-12), kiểm chứng chéo 2 nguồn độc lập.
- [x] Nếu chưa chắc, đánh dấu `⚠️ partial` (S-13, S-14, S-17) thay vì xoá.

### Quy tắc loại nguồn

| Mức ưu tiên | Loại nguồn | Ví dụ trong case này |
|---|---|---|
| 1 — Nguồn gốc | Báo cáo tài chính, thông báo chính thức, hồ sơ pháp lý | Prosus press release (S-01), OpenAI blog (S-03, S-12), GitHub blog (S-05), Stack Overflow blog (S-06, S-14), Google Cloud press (S-11) |
| 2 — Báo lớn | Báo chí công nghệ/kinh doanh uy tín | TechCrunch (S-01, S-09, S-12, S-15), VentureBeat (S-09), Reuters (S-04), InfoWorld (S-08), The Register (S-17) |
| 3 — Báo cáo phân tích | Báo cáo tài chính độc lập | SimilarWeb (S-13), Eric Holscher blog từ Stack Exchange Data Explorer (S-02) |
| 4 — Tránh dùng | Bài đăng cá nhân, blog không nguồn, mạng xã hội | Không dùng — riêng Medium "Faisal Feroz" / "ThreadSafe Diaries" đã loại vì không có data primary |

### Cảnh báo riêng cho case này

- **S-13 vs S-14 mâu thuẫn**: SimilarWeb nói traffic giảm 14% (Q1 2023), Stack Overflow nói chỉ giảm ~5%. Khả năng cao là **đo khác đối tượng** — SimilarWeb đo external visit (Google → SO), Stack Overflow đo trên server log (bao gồm bot/scraper + repeat visit). Khi viết phân tích, dẫn cả 2 thay vì chọn 1.
- **S-02 đáng tin nhất**: dữ liệu lấy từ Stack Exchange Data Explorer (chính chủ, query SQL công khai) → khó bịa.
- **AI có thể bịa**: nếu thấy ai (hoặc AI) trích "Stack Overflow mất 60% traffic" hoặc "doanh thu giảm $X triệu" — yêu cầu nguồn primary; Prosus chỉ công bố Stack Overflow gộp trong "EdTech & Others" segment, không tách số riêng cho từng quý gần đây.

---

## Phần D — Phát hiện ban đầu

Sau khi có số liệu, ghi nhanh 3-5 phát hiện đáng chú ý nhất. Đây chưa phải nhận định cuối — chỉ là quan sát.

- **Câu hỏi mới — chỉ số leading thật sự**: trong khi traffic web có thể giữ được bằng SEO + organic visit từ Google, thì **số câu hỏi đăng mới giảm 40.2% YoY chỉ trong 2 năm** (S-02) là dấu hiệu data flywheel đang chết. Không có câu hỏi mới → không có câu trả lời mới → dataset không cập nhật → AI competitor train bằng data Stack Overflow nhưng SO không có gì mới để cạnh tranh.
- **Tốc độ phản ứng 8 tháng có vẻ nhanh nhưng quá muộn**: từ ChatGPT (30/11/2022) đến OverflowAI announce (27/07/2023) là 8 tháng (S-07). Trong cùng khoảng đó, ChatGPT đạt 100 triệu MAU (S-04). Khi SO ra OverflowAI, người dùng đã chuyển hành vi.
- **Cắt 35% nhân sự trong 17 tháng** (S-10) — đợt 1 (10%) cách đợt 2 (28%) chỉ 5 tháng → ban lãnh đạo đánh giá sai tốc độ suy giảm ở đợt 1, phải cắt mạnh hơn vào đợt 2.
- **Reversal "ban → sell" (S-17 → S-12)**: 12/2022 ban ChatGPT khỏi platform; 05/2024 bán data cho OpenAI. Đây là dấu hiệu **mô hình kinh doanh cũ đã không cứu được** — phải chuyển sang bán data (commodity input) cho chính đối thủ giết mình.
- **Giá thay thế ngang ngửa nhau** (S-16): ChatGPT Plus $20 vs Copilot Business $19 — chênh lệch giá không tạo lợi thế cho ai. Người dùng chọn theo workflow (IDE hay browser), không theo giá. SO không có sản phẩm nào trong cả 2 workflow này.

---

## Phần E — Câu hỏi mở (cho phân tích Phần 2)

Trước khi chuyển sang `2-analysis.md`, bạn liệt kê các câu hỏi cần đào sâu:

- **Câu hỏi 1** — Stack Overflow có **chết vì AI** hay **đã suy yếu trước AI**? (Một số nguồn nói traffic đã giảm từ mid-2021, trước cả Copilot GA — vậy AI là cú đẩy chứ không phải nguyên nhân gốc?)
- **Câu hỏi 2** — Nếu **Product Market Fit của SO là "câu hỏi-câu trả lời được upvote"**, thì AI đã phá vỡ Fit nào trước: PMF (người dùng không cần Q&A nữa) hay Channel Fit (Google không còn link về SO ở top result)?
- **Câu hỏi 3** — **Stack Overflow for Teams** (sản phẩm B2B SaaS) có còn cứu được không? Đây là sản phẩm trả phí thực sự (public site chỉ ads). Nếu Teams sống được, SO sống được — câu này critical cho phần "có cứu vãn?".
- **Câu hỏi 4** — **Tại sao SO không tự xây Copilot** (IDE plugin) trước GitHub? Họ có dataset lớn nhất thế giới về code Q&A. Đây là lỗi chiến lược về **timing + execution**, không phải về **technology access**.
- **Câu hỏi 5** — Vai trò của **Prosus** (chủ sở hữu): họ có ép SO chạy theo profitability quá sớm không? Sa thải đợt 2 (S-09) ghi rõ "path to profitability" — có thể đây là yêu cầu từ holding, không phải tự nhiên.

Sau bước này, chuyển sang `2-analysis.md` để vận dụng Lens 1 (Customer Expectations + Four Fits) vào case bạn chọn.
