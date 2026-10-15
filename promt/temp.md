# Bộ prompt tổng hợp để quần giống sản phẩm thật

Prompt dài nhiều yêu cầu dễ bị AI bỏ sót, nên mình chia làm **1 prompt chính** và **3 prompt sửa riêng**.

## Chuẩn bị ảnh đầu vào (quan trọng nhất)
Tải lên đủ 3 ảnh, **không dùng ảnh adidas**:
- **Ảnh 1**: ảnh sản phẩm gốc toàn thân quần (đã xoá vết bẩn nếu được)
- **Ảnh 2**: ảnh cận **patch túi** (chụp điện thoại, ánh sáng đều)
- **Ảnh 3**: ảnh cận **cạp quần + dây rút**

## Prompt chính (tạo ảnh mới)

```
Image 1 is the real product reference (full shorts). Image 2 is a close-up of the pocket patch. Image 3 is a close-up of the waistband and drawstring. Copy the product from these images EXACTLY. Do not redesign or simplify any detail.

Create a new photorealistic e-commerce photo of a male model wearing these shorts.

FRAMING:
- Crop from just above the navel down to the shoes. The top edge cuts across the lower part of the t-shirt. Absolutely no face, head, neck, chest or shoulders visible.
- Camera at hip height, slightly angled from the front-left, vertical portrait 3:4.

POSE (artistic, relaxed, natural):
- Body turned in a gentle three-quarter angle, but both front zip pockets and both patches stay clearly visible.
- His right hand (left side of image) hangs loosely beside the thigh, fingers slightly curled, away from the pocket.
- His left hand (right side of image) rests with only the thumb hooked at the pocket opening, so the patch on that pocket is NOT covered.
- Weight on the left leg (straight), right leg slightly forward with a soft bent knee, feet close together with toes slightly outward.

SHORTS (must match the references exactly):
1. Fabric and color: warm matte chocolate brown double-knit, no shine, no grey tint, soft natural folds, visible side-seam and hem stitching.
2. Fit: relaxed, boxy, wide-leg, hem just above the knee, legs hanging loosely away from the thighs.
3. Waistband: wide elastic waistband with 3 to 4 rows of soft gathered ruching and natural wrinkles.
4. Drawstring: thick, solid black, round braided cord, tied in a small neat bow at the center, no eyelets, two short metal-tipped ends hanging only a few centimeters below the bow.
5. Pockets: two diagonal front zip pockets near the side seams, black zipper pulls.
6. Patch on EACH pocket (copy Image 2): a rectangular NAVY BLUE rubberized patch, a thin brown perforated mesh strip directly above it, and a thin WHITE stitch line beside it. No yellow or gold lines. Same size and position on both pockets.
7. No logos, no text, no center front seam, no extra pockets or details.

STYLING:
- Plain solid grey-purple t-shirt, slightly loose, hem draping naturally over the waistband with soft curved edges and small wrinkles.
- Plain white crew socks and plain white minimalist sneakers. No logos, no stripes, no text or brand marks anywhere.
- Natural leg skin with fine, soft leg hair, subtle highlights on knees and shins.

BACKGROUND AND LIGHT:
- Seamless smooth light blue-grey studio backdrop, soft diffused light from the front-left, a short soft shadow under the feet and a small darker contact shadow under each shoe sole.

Photorealistic, commercial fashion photography, sharp detail, no watermark.
```

## Prompt sửa riêng (chỉ dùng khi cần)

**Sửa patch** (kèm ảnh cận patch):
```
Image 1 is the photo to edit. Image 2 is a close-up of the real pocket patch.
Edit ONLY the pocket patches. Replace them with the patch in Image 2: rectangular navy blue rubberized patch, thin brown perforated mesh strip directly above, thin white stitch line beside it. Remove any yellow or gold line. Make both patches visible, same size and position. Keep everything else identical.
```

**Sửa dây rút và cạp** (kèm ảnh cận cạp):
```
Image 1 is the photo to edit. Image 2 is a close-up of the real waistband and drawstring.
Edit ONLY the waistband and drawstring to match Image 2: a wide elastic waistband with 3 to 4 rows of gathered ruching, and a thick solid black round braided drawstring tied in a small bow with two short metal-tipped ends. Keep everything else identical.
```

**Sửa màu và form:**
```
Edit ONLY the shorts: make the color a warm matte chocolate brown with no grey tint, and the fit wide and boxy with the hem just above the knee, matching the reference. Keep everything else identical.
```

## Quy trình đề xuất
1. Chạy **prompt chính** 3 đến 4 lần, chọn ảnh có dáng đẹp và ít lỗi nhất.
2. Sửa **từng lỗi một**, mỗi lần chỉ một prompt sửa riêng.
3. Làm thủ công phần còn lại: **xoá ngôi sao Gemini**, thêm bóng tiếp xúc dưới giày nếu còn yếu, rồi **upscale lên tối thiểu 1500px**.

## Checklist đối chiếu trước khi đăng
Đặt ảnh AI cạnh ảnh sản phẩm thật và kiểm tra:
- [ ] Nâu chocolate ấm, không ngả xám hoặc đỏ
- [ ] Patch **navy** (không đen), có dải lưới nâu phía trên và chỉ **trắng** (không vàng)
- [ ] Thấy được cả hai patch, không bị tay che
- [ ] Dây rút đen trơn, dày, đầu dây ngắn bọc kim loại
- [ ] Cạp to, nhún nhiều hàng
- [ ] Ống rộng, dài ngang trên gối
- [ ] Không logo, chữ hay sọc nào trên tất, giày, áo
- [ ] Không còn biểu tượng ngôi sao

Nếu patch vẫn sai sau 2-3 lần, cách chắc nhất là sửa bằng Photoshop hoặc ghép patch cắt từ ảnh gốc. Chạy xong gửi ảnh lại, mình sẽ đối chiếu từng mục với checklist trên.