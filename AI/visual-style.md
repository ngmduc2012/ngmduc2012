# Phong cách hình ảnh cho bộ GitBook cá nhân

Trạng thái: **bản đề xuất v0.1**, chưa phải nhận diện đã được tác giả chốt. Ảnh My Peace là mẫu thử đầu tiên. Phản hồi của tác giả trong cuộc trò chuyện mới hơn luôn được ưu tiên.

## Hướng đề xuất: Sổ tay tĩnh

Minh họa biên tập bằng nét mực trên giấy ngà, gợi cảm giác ghi chép của một người đã thử và đang chia sẻ lại. Hình phải liên quan tới nội dung bài, có một trọng tâm và đủ khoảng trống để dễ nhìn trong GitBook.

Điểm nhận diện đề xuất: nét viền hơi không đều, mảng màu trầm, hạt giấy nhẹ và ba chấm vàng đất nhỏ. Ba chấm chỉ là chi tiết minh họa thử nghiệm, không thay cho logo.

Ảnh mẫu: [My Peace](../docs/vi/.gitbook/assets/my-peace-quiet-notebook-01.png).

## Phần giữ chung

- Nền giấy ngà `#F4EFE4`; nét mực xanh than `#303B38`.
- Một màu nhấn chính; vàng đất `#C99D50` dùng rất ít.
- Nét mực mảnh nhưng vẫn rõ ở chiều rộng điện thoại; mảng màu tương đối phẳng, không bóng như nhựa.
- Chất liệu giấy vừa đủ nhận ra; không làm hình bẩn, cũ hoặc khó nhìn.
- Mỗi ảnh truyền tải một ý. Không ghép nhiều biểu tượng công nghệ chỉ để lấp chỗ trống.
- Ảnh mở bài ưu tiên ngang 16:9. Hình giải thích chọn tỷ lệ theo nội dung.
- Không gắn chữ vào ảnh minh họa mở bài. Title và caption nằm trong Markdown để dùng chung ảnh cho VI/EN.
- Không yêu cầu mô phỏng tên một nghệ sĩ; mô tả chất liệu, nét, màu và bố cục.

## Điều chỉnh theo sản phẩm

Đây là các gợi ý cần kiểm tra bằng ảnh mẫu tiếp theo, chưa được xác nhận đồng bộ trên cả ba sản phẩm.

| Sản phẩm | Màu nhấn đề xuất | Chủ thể theo bài |
| --- | --- | --- |
| My Dev | Xanh đá `#57778A` | Module, dòng dữ liệu, công cụ hoặc bàn làm việc khi có liên quan |
| My Wong | Đất nung `#B87558` | Sổ ghi chép, vật dụng, cách sắp xếp hoặc công cụ đang được giới thiệu |
| Wong Coupon / My Peace | Xanh rêu `#607F6B` | Không gian thực hành, chuỗi hạt, sổ hoặc đồ vật gắn với nội dung |

Không bắt buộc vẽ sổ, cây hay điện thoại trong mọi bài. Giữ cách thể hiện chung và thay chủ thể theo ý bài.

## Phân biệt minh họa và bằng chứng

Ảnh AI dùng để minh họa ý tưởng hoặc không khí. Khi cần chỉ thao tác, chứng minh kết quả, mô tả giao diện, dùng screenshot thật. Không tạo màn hình giả rồi trình bày như giao diện sản phẩm.

Sơ đồ kỹ thuật có nhãn chính xác nên dùng Mermaid hoặc vector có thể chỉnh sửa. Không bắt công cụ tạo ảnh đảm nhiệm chữ nhỏ, code, biểu đồ số liệu hay chi tiết API cần đúng tuyệt đối.

Với nội dung Phật học, không suy diễn công dụng tu tập hoặc kết quả tinh thần từ hình ảnh. Chỉ thêm nhân vật hay biểu tượng tôn giáo khi chủ đề và yêu cầu thực sự cần.

## Cách tạo và kiểm tra ảnh tiếp theo

1. Đọc đoạn bài cần minh họa, ghi một câu về ý chính của ảnh.
2. Chọn minh họa, screenshot thật hoặc sơ đồ theo mục đích.
3. Với minh họa AI, dùng công cụ imagegen tích hợp. Đưa ảnh mẫu đã được chọn làm tham chiếu phong cách khi công cụ hỗ trợ, thay vì chỉ lặp tên phong cách.
4. Giữ bảng màu và chất liệu; đổi chủ thể, số lượng vật và bố cục để đúng bài. Tạo một mẫu trước khi làm cả bộ.
5. Xem ảnh thực tế: ý chính rõ, vật không méo, không chữ rác, không UI giả, không chi tiết thừa át chủ thể. Kiểm tra ở chiều rộng điện thoại và trên trang sáng/tối.
6. Lưu asset trong repository, giữ ảnh gốc và prompt. VI/EN dùng cùng ảnh, có alt text và caption đúng ngôn ngữ.
7. Chỉ ghi trạng thái phong cách đã chốt khi có lựa chọn của tác giả. Việc tạo ảnh không tự cho phép sửa logo hoặc đổi toàn bộ nhận diện.

Nếu công cụ tích hợp không dùng được, báo giới hạn. Không tự chuyển sang dịch vụ/API tốn phí khác.

## Mẫu prompt

```text
Use case: illustration-story
Asset type: [article hero / concept illustration]
Purpose: [one sentence, drawn from the article]
Subject: [only the objects needed for that purpose]
Style: restrained editorial ink illustration, warm ivory paper, slightly irregular thin charcoal-green contours, muted flat washes, subtle paper grain
Palette: ivory #F4EFE4, charcoal-green #303B38, [product accent], a small amount of ochre #C99D50
Composition: [aspect ratio], one clear focal group, broad breathing room, readable at mobile size
Reference: [selected reference image; use for style, not for copying the scene]
Text: none; headings and captions are outside the image
Avoid: logos, watermarks, fake app UI, illegible labels, glossy 3D, excessive grain, irrelevant decoration
```

## Ảnh thử My Peace ngày 16/10/2026

- Công cụ: imagegen tích hợp; không dùng CLI/API fallback.
- Asset: `my-peace-quiet-notebook-01.png`, 1672 × 941, PNG.
- Vai trò: minh họa mở bài My Peace và landing Wong Coupon; không phải screenshot.
- Nhận xét khi xem ảnh: nét mực, giấy ngà, màu xanh rêu và ba chấm vàng đã hiện rõ. Công cụ thêm một chén trà ngoài chủ thể trong prompt; cần tác giả đánh giá chi tiết này có hợp hướng mong muốn không.
- Các ảnh My Dev/My Wong chưa được tạo, nên chưa khẳng định cả bộ đã nhất quán.

Prompt đã chạy:

```text
Use case: illustration-story
Asset type: wide editorial hero illustration for a Vietnamese personal article introducing My Peace, a Buddhist chanting counter Android application.
Primary request: Create one original, restrained illustration in the proposed house style "Quiet Notebook / So tay tinh". This is a style proof and usable article illustration, not an app screenshot or a religious promise.
Scene/backdrop: warm ivory uncoated paper, subtle fine paper grain. A quiet everyday desktop seen from a shallow overhead angle: a small loop of wooden chanting beads, an open cream notebook with blank pages, a modern phone placed face down, and a small single leafy stem at the edge. Arrange these as a single calm visual group with broad breathing room.
Style/medium: editorial ink drawing with slight natural line irregularity, thin dark charcoal-green contours and flat muted sage washes; subtle risograph-like ink grain, carefully designed simple forms, no photorealism and no glossy 3D.
Composition/framing: landscape approximately 16:9. One main cluster in the central lower two-thirds, generous negative space above and at edges. The bead loop and curved line of the stem gently echo an incomplete circle. Add exactly three tiny ochre printed dots as a restrained recurring editorial motif near one outer edge, away from the objects. No panel grid.
Palette: ivory #F4EFE4 dominant, charcoal-green #303B38 linework, muted sage #607F6B secondary, ochre #C99D50 very sparingly. Paper should feel light and readable even in a dark GitBook page.
Mood: quiet, personal, grounded, contemporary and warm, like an author's carefully kept practice notebook.
Constraints: no words, no letters, no numerals, no logo, no signature, no watermark, no invented app UI, no fake screenshot, no status bars, no Buddha/deity figure, no halo, no magical effects, no ornamental mandala, no ornate frame, no gradient glow, no stock-photo aesthetic. The phone back is plain and unbranded. No humans or hands. Make the composition distinctive through the hand-inked contours, limited palette and small three-dot motif rather than excess decoration.
```

