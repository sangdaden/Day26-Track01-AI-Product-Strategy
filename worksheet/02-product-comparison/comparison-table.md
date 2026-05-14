---
artifact: comparison-table — Bảng so sánh 8 chiều (freestyle research)
bai-tap: 2 — Phân tích sản phẩm AI (nhóm)
phase: Pre-test research + post-test verification
input: prompts/07-product-comparison.md + group-members.md
nop-cuoi: Không bắt buộc — file freestyle hỗ trợ slide deck
status: ⚠️ DỰ ĐOÁN ban đầu dựa trên public knowledge (cập nhật 05/2026) — nhóm phải VERIFY bằng test thật và sửa từng dòng sau khi có observation + screenshot
---

# Bảng so sánh 8 chiều — NotebookLM vs Claude Projects

**Ngành**: D — Nghiên cứu
**Sản phẩm A**: NotebookLM (Google) — <https://notebooklm.google.com>
**Sản phẩm B**: Claude Projects (Anthropic) — <https://claude.ai>
**Nhiệm vụ chung**: upload 3 PDF (TechCrunch SO sa thải / Eric Holscher SO decline / OpenAI partnership blog) → yêu cầu tóm tắt 500 từ tiếng Việt có citation
**Prompt chung**: xem `group-members.md` — paste y nguyên cho cả 2 sản phẩm, không điều chỉnh

---

## ⚠️ Lưu ý quan trọng trước khi đọc

Bảng dưới đây có **2 lớp**:

- **Lớp 1 — Thông tin sản phẩm (Chiều 5, 7)**: lấy từ trang giá chính thức + báo công nghệ uy tín — đáng tin cao nếu URL còn live.
- **Lớp 2 — Đánh giá kết quả test (Chiều 1, 2, 3, 4, 6, 8)**: **đây là dự đoán** dựa trên thiết kế đã biết của 2 sản phẩm. **PHẢI verify sau khi test thật**. Nếu thực tế khác, sửa lại bảng + ghi rõ "đã verify khi test" để slide deck có credibility.

---

## Bảng so sánh 8 chiều (dự đoán pre-test)

| # | Chiều | NotebookLM (A) | Claude Projects (B) | Thắng (dự đoán) |
|---|---|---|---|---|
| 1 | **Input — hiểu prompt** | Hiểu đúng prompt tiếng Việt; NotebookLM bị ràng buộc "chỉ trả lời từ sources" → nếu prompt yêu cầu thông tin ngoài 3 PDF, sẽ từ chối hoặc nói "không có trong sources" | Hiểu đúng prompt; có thể tự thêm context từ Claude general knowledge nếu prompt không cấm — đôi khi blur ranh giới "trong PDF" vs "kiến thức nền" | **Tương đương cho prompt này** (cả 2 hiểu yêu cầu) — nhưng A nghiêm ngặt hơn về "chỉ từ source" |
| 2 | **Output quality — tóm tắt 500 từ** | Output thường ngắn hơn yêu cầu (~350-450 từ), conservative, sát source. Ít hallucination vì kiến trúc RAG nghiêm. | Output thường đúng độ dài (~500 từ), văn phong mượt hơn, đôi khi thêm nhận định không có trong source (nếu không prompt rõ "chỉ dùng PDF") | **B thắng về văn phong + độ dài; A thắng về độ trung thực với source** → phụ thuộc use case |
| 3 | **Citation / Source** | **Citation inline cấp đoạn** — mỗi câu có nút số click được, jump thẳng vào đoạn PDF nguồn. Đây là điểm mạnh signature của NotebookLM. | Có thể cite (kèm tên file + đoạn) nếu prompt yêu cầu; KHÔNG có UI inline click-jump tự động — phải đọc citation text + tự tìm trong PDF | **A thắng rõ** — citation là feature gốc của NotebookLM, Claude Projects yếu hơn ở UI citation |
| 4 | **Speed** | Thường 10-25s cho query phức tạp trên 3 PDF (do RAG retrieval + grounding) | Thường 15-30s cho query tương tự (do reasoning Claude Sonnet/Opus + context lớn) | **Tương đương** — chênh ~5-10s không đủ ý nghĩa với use case research (không phải chat realtime) |
| 5 | **UI / Interaction** | UI chuyên biệt cho research: source pane bên trái, chat pane giữa, studio pane phải (Audio Overview, Mind Map, FAQ, Briefing Doc, Study Guide). Multi-modal output ngoài text. | UI là chat đơn giản (như Claude.ai); Project sidebar quản lý files + custom instructions; KHÔNG có audio/mind map. Có Artifacts cho output structured. | **A thắng cho research workflow** — multi-modal output cùng UI structured; **B thắng cho creative/coding workflow** — Artifacts mạnh hơn |
| 6 | **Tiếng Việt** | Tiếng Việt tự nhiên (powered by Gemini); citation và label UI một số chỗ vẫn EN. Audio Overview tiếng Việt đã được hỗ trợ (cập nhật 2025-2026). | Tiếng Việt rất tự nhiên (Claude vốn mạnh ngôn ngữ); toàn UI có thể chuyển sang VN; văn phong "người Việt hơn" theo nhiều bài đánh giá. | **B thắng nhẹ** về văn phong VN — nhưng cả 2 đều dùng được; cần verify với test thật vì khác biệt nhỏ |
| 7 | **Pricing / Giới hạn** | **Free tier**: rộng — đủ cho use case này. **Plus**: $7.99/tháng (Google AI Plus) — 200 notebooks, 100 sources/notebook, 200 chat/ngày, 6 Audio Overviews/ngày. **Pro**: $19.99/tháng (Google AI Pro). | **Không có free tier cho Projects** — phải có **Pro $20/tháng** mới dùng được Projects. **Team**: $25-30/user/tháng (min 5 users). 20 files / chat, 30MB / file. | **A thắng rõ về pricing** cho cá nhân/sinh viên — free tier đủ; B đòi phải trả $20/tháng từ ngày đầu |
| 8 | **Tổng cảm nhận** | Cảm giác "thư viện AI" — sản phẩm built-for-research; quy trình tự nhiên cho upload nhiều PDF + ask + cite. | Cảm giác "trợ lý đa năng" — Projects là wrapper trên Claude; mạnh suy luận, yếu UX research-specific. | **A best for**: "tôi cần ground-truth từ docs cụ thể, cite chính xác, không hallucinate". **B best for**: "tôi cần phân tích sâu, kết hợp doc + reasoning, output structured (artifacts/code)". |

---

## Nguồn cho thông tin sản phẩm (Lớp 1)

### Chiều 5 — UI (nguồn chung)

- NotebookLM Wikipedia: <https://en.wikipedia.org/wiki/NotebookLM> — features Audio Overview, Mind Map, FAQ, Briefing Doc, Study Guide
- DigitalOcean — "What Is NotebookLM? Features and How to Use It in 2026": <https://www.digitalocean.com/resources/articles/what-is-notebooklm>
- Anthropic Claude pricing page: <https://claude.com/pricing> — feature list Projects

### Chiều 7 — Pricing & limits (verified 05/2026)

- **NotebookLM**:
  - Plans page chính thức: <https://notebooklm.google/plans>
  - "NotebookLM Plus is now available in Google One AI Premium" (Google blog, 02/2025): <https://blog.google/feed/notebooklm-google-one/>
  - FelloAI summary 2026: <https://felloai.com/notebooklm-pricing/> — giá Plus $7.99, Pro $19.99, Ultra $249.99
- **Claude Projects**:
  - Claude pricing page chính thức: <https://claude.com/pricing>
  - FelloAI Claude pricing 2026: <https://felloai.com/claude-pricing/> — Pro $20/tháng, Team $25-30/user/tháng (min 5)
  - File upload limits: 20 files / chat, 30MB / file (Pro/Team tier)

---

## Nhận xét tổng thể (3-5 câu — pre-test draft)

Cho nhiệm vụ **tóm tắt 3 PDF với citation chính xác**, NotebookLM (A) **thắng rõ** ở 3 chiều quyết định: (1) citation inline click-jump là feature gốc, không phải add-on; (2) kiến trúc RAG nghiêm ràng buộc model chỉ dùng source upload — giảm hallucination; (3) free tier đủ dùng — không cần trả tiền để test. Claude Projects (B) thắng ở văn phong tiếng Việt + độ dài output sát yêu cầu + chiều sâu phân tích — nhưng **trả giá bằng paywall $20/tháng và citation yếu hơn**.

**Verdict per persona**:

- **Sinh viên / researcher mới**: chọn NotebookLM — free, citation tốt, audio overview giúp đa giác quan.
- **Professional cần output dài + reasoning sâu**: chọn Claude Projects — văn phong tốt hơn, Artifacts mạnh cho output structured.
- **Nhóm Lab 2 chấm điểm cao**: nên dùng NotebookLM cho nhiệm vụ này vì citation là tiêu chí chấm.

---

## Phản biện (3 câu stress-test)

1. **Hidden trade-off**: NotebookLM "thắng citation" nhưng có thể **không tổng hợp được luận điểm xuyên 3 PDF tốt như Claude** — vì RAG retrieve từng chunk, đôi khi mất context tổng thể. **Cần verify**: tóm tắt của NotebookLM có "đan xen" được số liệu từ 3 PDF khác nhau không, hay chỉ liệt kê từng PDF?
2. **Time-bound**: So sánh này áp dụng 05/2026. Claude đã có hint về việc thêm citation UI (Claude 4.7 có feature citations native qua API). Trong 6 tháng tới, citation gap có thể đóng. NotebookLM cũng đang thêm "Deep Research" — sẽ thay đổi cảnh quan.
3. **Different segment**: Test cho persona **sinh viên VN làm research case study**. Cho persona **legal counsel cần precise citation trong contract review** — NotebookLM thắng còn mạnh hơn (citation là deal-breaker). Cho persona **creative writer cần brainstorm từ source**, Claude Projects thắng vì flexibility cao hơn.

---

## Bias check

- **Bias 1**: Nếu nhóm có thành viên đã dùng Claude lâu (Claude Projects ra 06/2024), có thể đánh giá quá cao văn phong VN của Claude. Đối phó: cho thành viên ít quen với cả 2 chấm độc lập rồi đối chiếu.
- **Bias 2**: Cả 2 sản phẩm thay đổi nhanh (NotebookLM thêm feature gần như hàng tháng; Claude release model mới mỗi vài tháng). Bảng này valid cho **05/2026** — note rõ ngày test trên slide.
- **Bias 3**: Chọn 3 PDF từ Lab 1 → có thể tự dưng có advantage cho 1 sản phẩm vì content "khớp" với training data. Đối phó: test thêm 1 PDF "lạ" (vd: 1 paper khoa học VN ít người dùng) để kiểm tra cross-domain.

---

## Frameworks lecture được áp dụng vào bảng so sánh

### 7 Customer Expectation Shifts

- **Shift 1 — Do the work for me**: B (Claude Projects) đáp ứng tốt hơn — output dài + chi tiết hơn, ít cần edit. A (NotebookLM) vẫn để user "tự đọc citation".
- **Shift 7 — Tool sees what I'm doing**: A thắng — đọc source upload là context-aware mặc định; B cần user explicitly add files vào project.

### Niche Down (Lens 2)

- **A — NotebookLM**: **Niche rõ ràng** — "research notebook on your own sources". Mọi feature (Audio Overview, Mind Map, FAQ, Briefing) đều phục vụ research. Không cố làm general chatbot.
- **B — Claude Projects**: **Niche yếu hơn** — Projects là wrapper bên trên Claude chat. Có thể dùng cho coding, writing, research — không có UX riêng cho research.

### AI Feature Map (Lens 3) — User Value × User Alignment × Business Value

- **A — NotebookLM**: Sweet spot — User Value cao (research workflow đúng pain point), User Alignment cao (Google brand + free tier), Business Value vừa (Google bundle để giữ user trong AI Premium subscription).
- **B — Claude Projects**: Sweet spot vừa — User Value cao cho user đã trả Claude Pro; User Alignment cao với power user; Business Value cao (drive Pro/Team subscription).

### Defensibility / Moat (Lens 4)

- **A — NotebookLM**: Moat = **Distribution** (Google account + Workspace + AI Premium bundle) + **Data flywheel yếu** (user upload là personal, không feed back model). Moat trung bình.
- **B — Claude Projects**: Moat = **Model quality** (Claude Opus 4.7 + 1M context) + **Brand trong dev/professional** + **API moat** cho enterprise. Moat mạnh hơn về long-term defensibility.

---

## Liên hệ Lab 1 case Stack Overflow

Cả 2 sản phẩm đều "có thể disrupt Stack Overflow" theo cách khác nhau:

- **NotebookLM** thay use case "upload doc + ask question" — nhưng SO Q&A là public, không phải personal docs → ít overlap trực tiếp.
- **Claude Projects** thay use case "tích hợp kiến thức tổ chức + ask" — overlap **trực tiếp với Stack Overflow for Teams** (sản phẩm B2B của SO). Claude Projects rẻ hơn ($20 vs SO Teams ước $6-12/user nhưng cần thêm hạ tầng), flexible hơn, không cần dataset Q&A có sẵn.

→ **Bài học cho slide S5.8**: nếu Stack Overflow là nạn nhân của AI disruption ở Lab 1, thì **Claude Projects + NotebookLM chính là 1 phần thế hệ AI tool đang nuốt tiếp B2B knowledge tool** (Confluence, SharePoint, SO Teams). Lab 2 chính là "test mặt bên kia của câu chuyện Lab 1".

---

## TODO sau khi test thật

- [ ] Cập nhật Chiều 1 (Input) với observation thật từ cả 2 sản phẩm
- [ ] Cập nhật Chiều 2 (Output Quality) với số từ chính xác, số lỗi cụ thể, số hallucination đếm được
- [ ] Cập nhật Chiều 3 (Citation) với số nguồn click được vs tổng, % chính xác
- [ ] Cập nhật Chiều 4 (Speed) với giây đo thực tế cho từng query
- [ ] Cập nhật Chiều 6 (Tiếng Việt) với ví dụ câu cụ thể từ output mỗi sản phẩm
- [ ] Chụp đủ 6 screenshot mỗi sản phẩm theo template `screenshots/README.md`
- [ ] Đổi status frontmatter từ "DỰ ĐOÁN" → "ĐÃ VERIFY" + ngày test
- [ ] Paste bảng + nhận xét vào slide deck S2 (Workflow) + S5 (Verdict)
