# derival-campaign — luật cho Claude

Repo **PUBLIC** chỉ chứa sản phẩm (mp4, ảnh) của studio Derival. Mọi luật nội dung, công cụ, chiến lược ở repo
`derivallcc/derival-studio` (đọc `CLAUDE.md` ở đó trước khi làm nội dung).

- Ghi vào đây **chỉ** bằng `scripts/archive_run.py` của studio (nó cập nhật `media/<CT>/` và `index.csv` cùng lúc).
- Không bao giờ đưa vào: khoá/token, `secrets/`, caption nội bộ, bản tin D-family, điểm barem, ghi chú admin, `post_kit.md`,
  số tài khoản, lệnh đang mở, dữ liệu cá nhân, file dự án (`projects/`), bản nháp nội bộ không định giao.
- File ≤ 25 MB. Không sửa hay xoá file cũ đã gửi link (link trong bản tin phải sống); phiên bản mới = file mới `_v<n+1>`.
  Muốn gỡ một video khỏi công khai: hỏi người dùng trước (đã có link trong nhóm và lịch sử git vẫn giữ file).
- Commit `<CT>_<v>: <loại>` lên `main`.
