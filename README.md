# bye-bye-tamnc 🌻

Thiệp chia tay anh **Nguyễn Chí Tam** — tông vàng cam, dựa trên template [anhnt-24/bye-bye-namtlv](https://github.com/anhnt-24/bye-bye-namtlv).

## Thả ảnh vào `images/`

| Vị trí | Tên file |
|---|---|
| 8 khung lớn quanh màn hình (desktop ≥1024px) | `khung-1.jpg` … `khung-8.jpg` |
| 4 ảnh dán trong thư | `thu-1.jpg` … `thu-4.jpg` |
| 2 sticker hai bên (PNG nền trong, màn ≥900px) | `sticker-trai.png`, `sticker-phai.png` |

Khung nào chưa có ảnh sẽ hiện 📷 kèm tên file cần thả. Dùng đuôi khác (`.png`, `.jpeg`) thì sửa `src` trong `index.html`.

## Sửa chữ
- Nội dung thư: tìm `✏️ Sửa nội dung thư` trong `index.html`.
- Chú thích ảnh: các thẻ `<figcaption>`.
- Nhạc nền: thay `music.mp3`.

## Hiệu ứng
Tia nắng xoay + quầng sáng thở, đom đóm bay lên, hoa/lá rơi, phong bì bồng bềnh có vệt sáng quét + con dấu toả vòng sáng,
pháo hoa + confetti khi mở thư, đoạn thư hiện dần, tiêu đề ánh vàng, ảnh nghiêng 3D theo chuột, lightbox chuyển ảnh ← →,
vệt lấp lánh theo con trỏ, pháo hoa nhỏ khi bấm ra ngoài. Tôn trọng `prefers-reduced-motion`.

## Chạy
Mở `index.html`, hoặc `python3 -m http.server` rồi vào http://localhost:8000. Deploy tĩnh được lên GitHub Pages / Vercel.
