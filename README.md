# derival-media

Kho **ảnh, video và nội dung do Claude tạo ra** cho studio Derival — dùng trên Facebook, TikTok, Instagram, YouTube, LinkedIn và các
kênh Telegram/Zalo của Derival. Công cụ, chiến lược, kịch bản, lịch sử tạo nằm ở repo studio (private); studio **không** lưu video/kết quả
dựng mà **tham chiếu** kho này (`index.csv`, tờ khung hình) để nội dung mới không trùng lặp, không nhàm chán.

## Cấu trúc

| Đường dẫn | Chứa gì |
|---|---|
| `media/<CT-xxxx>/<CT>_<v>.mp4` | Video đã giao (H.264, ≤ 25 MB) |
| `media/<CT-xxxx>/<CT>_<v>_frames.jpg` | Tờ 8 khung hình để xem nhanh |
| `media/<CT-xxxx>/<CT>_<v>_cover*.jpg`, `*.png` | Ảnh bìa, carousel, ảnh tĩnh |
| `index.csv` | Một dòng mỗi file: ngày, mã nội dung, phiên bản, loại, đường dẫn, dung lượng, sha256, thời lượng, link tải trực tiếp |

Link tải trực tiếp một video (không cần đăng nhập):
`https://raw.githubusercontent.com/derivallcc/derival-media/main/media/<CT>/<CT>_<v>.mp4`

File ở đây do `scripts/archive_run.py` của studio ghi. Có mặt trong repo **không** có nghĩa là đã duyệt đăng — trạng thái duyệt theo
dõi ở studio (`brain/content/registry.csv`).

## Lưu ý

Nội dung mang tính thông tin, không phải tư vấn đầu tư. Kết quả quá khứ không đảm bảo kết quả tương lai.
Video chỉ nói về lệnh đã đóng. © Công ty TNHH Derival — không dùng lại cho mục đích thương mại khi chưa được phép.
