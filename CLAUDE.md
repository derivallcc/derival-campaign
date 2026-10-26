# derival-media — luật cho Claude

Repo **PUBLIC** lưu ảnh/video/nội dung Claude tạo ra cho studio Derival (đổi tên từ `derival-campaign` ngày 25/10/2026). Studio đọc `index.csv` và `media/*/*_frames.jpg` ở đây để chống lặp nội dung. Mọi luật nội dung, công cụ, chiến lược ở repo
`derivallcc/derival-studio` (đọc `CLAUDE.md` ở đó trước khi làm nội dung).

- Ghi vào đây **chỉ** bằng `scripts/archive_run.py` của studio (nó cập nhật `media/<CT>/` và `index.csv` cùng lúc).
- **Mỗi sản phẩm có đủ thông tin đăng ở đây** (TD-018, 25/10/2026): `media/<CT>/<CT>_post.md` — caption 5 MXH + kênh/nhóm, giờ đăng, ảnh bìa,
  bình luận ghim, hashtag, câu miễn trừ. Bản tin Telegram gửi link file này. Studio không lưu kết quả.
- **Mỗi sản phẩm có kịch bản ở đây** (TD-023, 26/10/2026): `media/<CT>/<CT>_<v>_script.md` — lời đọc + chữ trên hình theo cảnh
  (bản công khai, không cột thiết kế nội bộ). Studio quét các file này và `_post.md` (`scripts/script_scan.py`) để nội dung mới không lặp lời, hook, câu chốt.
- Không bao giờ đưa vào: khoá/token, `secrets/`, bản tin D-family, điểm barem, ghi chú nội bộ (trạng thái chấm, "cần quyết"),
  số tài khoản, lệnh đang mở, dữ liệu cá nhân, file dự án (`projects/`), bản nháp nội bộ không định giao.
- File ≤ 25 MB. Không sửa hay xoá file cũ đã gửi link (link trong bản tin phải sống); phiên bản mới = file mới `_v<n+1>`.
  Muốn gỡ một video khỏi công khai: hỏi người dùng trước (đã có link trong nhóm và lịch sử git vẫn giữ file).
- Commit `<CT>_<v>: <loại>` lên `main`.
