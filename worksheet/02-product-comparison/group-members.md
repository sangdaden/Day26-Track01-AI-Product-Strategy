---
artifact: group-members — Danh sách thành viên nhóm Lab 2
bai-tap: 2 — Phân tích sản phẩm AI (nhóm)
phase: Khai báo nhóm
nop-cuoi: Có — bắt buộc (nộp kèm analysis-report.pdf)
---

# Thành viên nhóm Lab 2

Lab 2 làm theo nhóm 2 học viên. Mỗi học viên có 1 repo riêng (`Day26-MãHọcViên`), nhưng nội dung Lab 2 (slide deck + screenshots + research notes) là sản phẩm chung — mỗi học viên copy bản chung về repo cá nhân của mình.

File này khai báo 2 thành viên trong nhóm + phân công thực hiện.

---

## Danh sách thành viên

| # | Mã học viên | Họ tên đầy đủ | Phân công chính |
|---|---|---|---|
| 1 | 2A202600280 | Phan Thanh Sang | Test + chụp screenshot Sản phẩm A (NotebookLM); viết draft S1 (Product Moment) + S2 (Workflow); làm liên hệ Lab 1 case Stack Overflow ở S5.8 |
| 2 | 2A202600314 | [Trần Tiến Dũng] | Test + chụp screenshot Sản phẩm B (Claude Projects); viết draft S3 (Friction Audit) + S4 (Moat Check); chuẩn bị slide deck export PDF |

---

## Nhiệm vụ thử nghiệm chung

Cả 2 thành viên cùng test trên 2 sản phẩm **cùng 1 bộ input + cùng 1 prompt**: upload 3 file PDF về case "Stack Overflow bị ChatGPT disrupt" (lấy từ nguồn Lab 1 — TechCrunch sa thải, Eric Holscher decline data, OpenAI partnership), rồi yêu cầu mỗi sản phẩm tạo **bản tóm tắt 500 từ có dẫn nguồn cụ thể** (mỗi nhận định phải link về file PDF + đoạn nào).

Lý do chọn use case này: trùng pipeline thật của Lab 1 — research + tóm tắt + cite source — nên có thể đối chiếu chất lượng output với phân tích Lab 1 đã làm.

**Ngành chọn**: D — Nghiên cứu

**Sản phẩm A**: **NotebookLM** (Google) — <https://notebooklm.google.com>

**Sản phẩm B**: **Claude Projects** (Anthropic) — <https://claude.ai> (feature Projects, có trong gói Pro/Team)

### File PDF dùng chung cho cả 2 test

Cả 2 thành viên upload **cùng 3 PDF** sau (export từ URL Lab 1):

1. TechCrunch — "Stack Overflow cuts 28% of its staff" (17/10/2023) — bài về sa thải đợt 2
2. Eric Holscher — "Stack Overflow's decline" (21/01/2025) — phân tích dữ liệu giảm câu hỏi
3. OpenAI blog — "API Partnership with Stack Overflow" (06/05/2024) — bài thoả thuận data

### Prompt chung dùng cho cả 2 sản phẩm (không sửa giữa 2 lần test)

```text
Dựa trên 3 file PDF tôi đã upload, viết 1 bản tóm tắt 500 từ về case
"Stack Overflow bị disrupt bởi ChatGPT" theo cấu trúc:
1. Bối cảnh (100 từ)
2. Sự kiện gãy + số liệu cụ thể (200 từ)
3. Phản ứng của Stack Overflow (150 từ)
4. Nhận định cốt lõi (50 từ)

Mỗi số liệu hoặc nhận định phải có citation rõ ràng đến file PDF cụ thể
(tên file + đoạn nào / page nào nếu có).
Trả lời bằng tiếng Việt.
```

---

## Phân chia screenshot

- Sản phẩm A (NotebookLM) → **2A202600280 — Phan Thanh Sang** phụ trách chụp
- Sản phẩm B (Claude Projects) → **2A202600314 — [Trần Tiến Dũng]** phụ trách chụp

Mỗi sản phẩm chụp tối thiểu 6 ảnh theo `screenshots/README.md`:

- `product-A-1-entry.png` — trang chủ NotebookLM
- `product-A-2-input.png` — sau khi upload 3 PDF
- `product-A-3-output.png` — bản tóm tắt 500 từ trả ra
- `product-A-4-source.png` — phần dẫn nguồn (NotebookLM có inline citation click được)
- `product-A-5-pricing.png` — trang giá NotebookLM Plus / Google AI Premium
- `product-A-6-limit.png` — nếu gặp quota (ít khả năng vì free tier rất rộng)

Tương tự với product-B-* cho Claude Projects.

---

## Ghi chú

- Mỗi thành viên copy folder `02-product-comparison/` (đã hoàn thiện) vào repo cá nhân của mình.
- Slide deck `analysis-report.pdf` và `analysis-report-link.md` (nếu có) là sản phẩm chung — 2 thành viên cùng tên trong credits của slide deck.
- File `group-members.md` này phải giống nhau ở cả 2 repo cá nhân (cùng nội dung, cùng 2 mã học viên).
- **Thành viên 2 cần điền lại**: thay placeholder `2A202600314` và `[Trần Tiến Dũng]` bằng thông tin thật trước khi commit final.

---

## Cấu trúc Analysis Report — S5 mở rộng

Slide deck Analysis Report có 5 mục bắt buộc (S1 → S5). Mục S5 (Product Judgment) được mở rộng thành 8 mục con để bám sát 5 chiều phân tích định lượng (user base, tăng trưởng, doanh thu, moat, data flywheel) đã làm ở Lab 1 Phần B.

- **S5.1 Verdict** — mỗi sản phẩm xếp loại Strong / Promising / Weak / At Risk, kèm lý do 1 câu.
- **S5.2 User base + tăng trưởng** — số liệu công khai (MAU, DAU, paid users, growth rate) cho cả 2 sản phẩm + nguồn.
- **S5.3 Doanh thu / pricing power** — mức giá so với value cung cấp; ARR/MRR nếu công khai; pricing strategy (freemium, premium, enterprise).
- **S5.4 Moat phân tích** — đánh giá 5 loại moat (data / network / switching cost / brand / distribution) cho từng sản phẩm; moat nào mạnh, moat nào dễ bị copy.
- **S5.5 Data flywheel + feedback loop** — hành động người dùng nào feed lại model; loop có compounding không; sản phẩm có thu thập feedback systematically.
- **S5.6 Niche Down + AI Feature Map** — sản phẩm có niche rõ không; map User Value / User Alignment / Business Value cho từng sản phẩm.
- **S5.7 Spark → Loop → System** — mỗi sản phẩm đang ở giai đoạn nào; dự báo 12 tháng tới.
- **S5.8 Liên hệ Lab 1 case** — 2 sản phẩm có rủi ro disruption-style tương tự case Lab 1 không; bài học rút từ Lab 1 áp dụng được gì?

Nhóm bắt buộc xong S5.1, S5.6, S5.7, S5.8 (giữ nguyên yêu cầu cốt lõi như bản gốc). S5.2–S5.5 là phần mở rộng cho yêu cầu phân tích sâu — nhóm khá phải hoàn thành đủ; nhóm Đạt có thể chấp nhận ghi "không có nguồn công khai" cho 1-2 số liệu, miễn có ghi rõ.
