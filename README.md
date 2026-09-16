# bye-bye-tamnc 🌻

Thiệp chia tay anh **Nguyễn Chí Tam**, dựa trên template [anhnt-24/bye-bye-namtlv](https://github.com/anhnt-24/bye-bye-namtlv). Có 2 chế độ, chuyển bằng nút góc trên bên trái:

- **🌻 Nắng** (`index.html`) — phong bì, lá thư giấy kẻ, tông vàng cam.
- **🎮 Game** (`play.html` → `game.html`) — LMHT × PUBG:
  - `play.html`: **Giúp TamNC bắn hạ AnhNT** — game bắn súng góc nhìn thứ nhất (3D, Three.js). AnhNT đứng giữa đấu trường, thân 3D, **đầu là ảnh**; né qua lại, cà khịa anh Tam, nổi giận khi còn nửa máu. Bắn hạ xong tự sang hậu trận.
  - `game.html`: hậu trận — thẻ MVP, tổng kết trận (lấy số liệu trận vừa bắn), highlight, Honor, kênh chat, nút "Tốt rồi", thành tựu, kill feed.

## Thả ảnh vào `images/`

| Vị trí | Tên file |
|---|---|
| 8 khung lớn (bản Nắng) / 8 thẻ Highlight (bản Game) | `khung-1.jpg` … `khung-8.jpg` |
| 4 ảnh trong thư (Nắng) / ảnh chụp dưới kênh chat (Game) | `thu-1.jpg` … `thu-4.jpg` |
| 2 sticker hai bên (PNG nền trong, màn ≥900px) — chỉ bản Nắng | `sticker-trai.png`, `sticker-phai.png` |
| Ảnh đại diện thẻ MVP — chỉ bản Game | `avatar.jpg` |
| Đầu AnhNT trong game bắn (PNG đã tách nền; không có thì cắt tròn `anhnt.jpg`) | `anhnt.png` |

Khung nào chưa có ảnh sẽ hiện 📷 kèm tên file cần thả. Dùng đuôi khác (`.png`, `.jpeg`) thì sửa `src` trong `index.html`.

## Sửa chữ
- Nội dung thư: tìm `✏️ Sửa nội dung thư` trong `index.html`.
- Chú thích ảnh: các thẻ `<figcaption>`.
- Chữ bản Game (chỉ số, Honor, tin nhắn, kill feed): khối `✏️ NỘI DUNG` đầu `<script>` trong `game.html`.
- Câu thoại, máu, sát thương trong game bắn: khối `✏️ NỘI DUNG` trong `play.html`.
- Nhạc nền: thay `music.mp3`; bản Game ưu tiên `music-game.mp3` nếu có.

## Hiệu ứng
Tia nắng xoay + quầng sáng thở, đom đóm bay lên, hoa/lá rơi, phong bì bồng bềnh có vệt sáng quét + con dấu toả vòng sáng,
pháo hoa + confetti khi mở thư, đoạn thư hiện dần, tiêu đề ánh vàng, ảnh nghiêng 3D theo chuột, lightbox chuyển ảnh ← →,
vệt lấp lánh theo con trỏ, pháo hoa nhỏ khi bấm ra ngoài. Tôn trọng `prefers-reduced-motion`.

## Chạy
Mở `index.html`, hoặc `python3 -m http.server` rồi vào http://localhost:8000. Deploy tĩnh được lên GitHub Pages / Vercel.
