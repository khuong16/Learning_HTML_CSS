## Chương 1: Kiến thứ HTML cần nắm vững:

1. Thiết lập code editor cơ bản:

   - Các extensions nên cài:

   Prettier
   Material Icon Theme
   Live Server
   Bracket Pair Colorizer
   Highlight Matching Tag
   SCSS Intellisence
   htmltagwrap
   HTML to CSS Autocompletion
   HTML Snippets
   Live Server Preview
   Auto Complete Tag

   - Các extensions hay cho Chrome:

   Eye Dropper
   Page Ruler Redux
   VisBug

   - Trang web lấy ảnh miễn phí: Unsplash

2. Cấu trúc một file HTML cơ bản như thế nào ?

3. Các thẻ HTML cơ bản nên biết phần 1 ?

- Các thẻ cần nhớ: div, p, h1 - h6, a, img, ul, ol

4. Các thẻ HTML cơ bản nên biết phần 2.

- Thẻ sematic là những thẻ mới sinh ra ở html5 sau này.
- Giúp code gọn hơn và đẹp hơn, mạch lạc hơn rất nhiều.
- header, footer, aside, nav, main, section, article (sử dụng cho 1 bài viết nhỏ), iframe (nhúng video vô), span(đoạn văn bản ngắn), strong(in đậm), em(in nghiêng), b(in đậm), i(in nghiêng)

5. Thẻ inline và thẻ block khác nhau như thế nào ?

- Xem thẻ nào là thẻ nào là thẻ inline, thẻ nào là thẻ block thì sẽ có trang web để check: https://htmlreference.io/
- Thẻ inline sẽ có độ rộng bằng nội dung nó chứa
- Nếu nhiều thẻ inline thì nó sẽ nằm trên cùng 1 hàng với nhau.
- Thẻ inline bị hạn chế về CSS

- Thẻ block có độ rông full phần tử chứa nó.
- Nếu nhiều thẻ block nằm với nhau thì nó rớt xuống hàng.

6. Sự khác nhau giữa class và id:

- Custom Attribute: sử dụng cấu trúc data-\*
  (ví dụ: sử dụng href trong thẻ div, data-href)
- class: có thể trùng nhau, sử dụng cho nhiều phần tử giống nhau.
- id: duy nhất, chỉ có duy nhất 1 id đó (không được trùng nhau)
  VD: khi làm việc với form, input,...

7. BEM là gì ? Tìm hiểu BEM toàn tập.

- BEM(Block Element Modifier) là quy chuẩn đặt tên class.
  VD: Laptop : Block
  Keyboard, Mouse, Touchpad, Screen: Element
  Laptop big, Laptop small: Modifier for Block
  Small keyboard, small screen: Modifier for Element

      Block__Element--modifier
      Block--modifier
      Block__Element

      laptop
      laptop__keyboard, laptop__touchpad, laptop__screen
      laptop--small, laptop--expensive, laptop--big
      laptop__touchpad--smouth, laptop__screen--scale

      tiêu đề: title
      danh mục: category

8. Thực hành phân tích giao diện cơ bản với BEM
9. Bài tập chương 1
10. Giới thiệu bài tập chương 1 phần 1.
11. Nắm vững Emmet cơ bản trong VSCode.

## Chương 2: Kiến thức CSS cơ bản phần 1

- CSS reset là gì ? Tại sao phải dùng reset CSS ?
- Cấu trúc của 1 đoạn code trong CSS như thế nào ?
- Tìm hiểu thuộc tính color, các giá trị về màu sắc cần nắm vững.
- Nắm vững kiến thức về kích thước trong CSS.
- Làm hình nền với thuộc tính về background
- Các đơn vị trong css nên biết.
- Đơn vị em và rem khác nhau như thế nào ?
- Thuộc tính về border cơ bản.
- Nắm rõ thuộc tính margin
- Hiểu về thuộc tính padding.
- Tìm hiểu về box-sizing trong CSS.
- Tìm hiểu thuộc tính display.
- Các thuộc tính liên quan tới font cơ bản.
- Các thuộc tính liên quan tới chữ bạn cần biết.
- Tìm hiểu thuộc tính cho hình ảnh.
- Pseudo là gì ? Các pseudo cơ bản người mới học nên biết.
- Bài tập chương 2 phần 1
- Bài tập chương 2 phần 2

## Chương 3: Kiến thức CSS cơ bản phần 2

- Cách làm hình nền gradient, chữ gradient trong CSS
- Hiển thị 2 hình nền với background-image
- Caniuse là gì ? và tại sao bạn nên biết.
- Sự khác nhau giữa 3 thuộc tính opacity, display, visibility
- Tìm hiểu về shadow trong CSS.
- Sự dụng biến trong CSS như thế nào ?
- Hiểu rõ về độ ưu tiên trong CSS, xác định độ ưu tiên trong CSS đơn giản với VSCode.
- Nắm vững kiến thức về child selectors
- Nắm vững kiến thức về type selectors
- Thành thạo combinators trong CSS
- Tìm hiểu thêm các selectors nâng cao
- Nắm vững thuộc tính transition cơ bản.
- Bài tập chưỡng 3.

## Chương 4: Kiến thức CSS nâng cao

- Thuộc tính transform để làm gì ? Tìm hiểu các giá trị hay dùng của transform.
- Tìm hiểu thuộc tính position relative.
- Master thuộc tính tính position absolute.
- Hiểu rõ position fixed hoạt động.
- Thực hành với thuộc tính position bài 1.
- Thực hành với thuộc tính position bài 2.
- Thực hành với thuộc tính position bài 3.
- Thực hành với thuộc tính position bài 4.
- Hiểu và nắm tốt pseudo :before và :after khó nhằn trong CSS.
- Thực hành với pseudo before và after bài 1.
- Thực hành với pseudo before và after bài 2.
- Thực hành với pseudo before và after bài 3.
- Thực hành với pseudo before và after bài 4.
- Tại sao before và after quan trọng và lưu ý khí làm với transform.
- Animation là gì ? Tìm hiểu và nắm vững kiến thức về animation cơ bản.
- Thực hành với animation bài số 1.
- Thực hành với animation bài số 2.

## Chương 5: Flexbox toàn tập

- Flexbox là gì ? Giới thiệu về Flexbox
- Flexbox toàn tập phần 1
- Flexbox toàn tập phần 2
- Flexbox toàn tập phần 3.
- Các thủ thuật chia layout hay mà bạn nên biết khi dùng Flexbox.
- Cách vẽ tam giác bằng CSS và cách nó hoạt động.
- Sass là gì ? Giới thiệu và cài đặt
- Tìm hiểu và nắm cơ bản kiến thức về Sass cho người mới.
- Các lỗi hay gặp khi cài đặt Sass và cách khắc phục.
- Thực hành code giao diện dropdown phần 1
- Thực hành code giao diện dropdown phần 2
- Thực hành code giao diện dropdown phần 3
- Thực hành code giao diện đơn giản số 1 với flexbox phần 1.
- Thực hành code giao diện đơn giản số 1 với flexbox phần 2.
- Thực hành code giao diện đơn giản số 1 với flexbox phần 3
- Responsive là gì ? Giới thiệu về responsive toàn tập.
- Thực hành code giao diện đơn giản số 1 sử dụng responsive.
- Thực hành code giao diện đơn giản số 2
- Thực hành code giao diện đơn giản số 3 phần 1
- Thực hành code giao diện đơn giản số 3 phần 2
- Thực hành code giao diện đơn giản số 4 phần 1
- Thực hành code giao diện đơn giản sô 4 phần 2
- Thực hành code giao diện đơn giản số 4 phần 3

## Chương 6: Các thẻ HTML về Form, Table.

- Tìm hiểu các thẻ về Form phần 1
- Tìm hiểu các thẻ về Form phần 2.
- Nguyên lý hoạt động và cách làm custome checkbox.
- Nguyên lý hoạt động và cách làm custom radio.
- Nguyên lý hoạt động và cách làm custom input file.
- Nguyên lý hoạt động và cách làm custom checkbox toggle.
- Thực hành code giao diện form số 1 phần 1.
- Thực hành code giao diện form số 1 phần 2.
- Thực hành code giao diện form số 1 phần 3.
- Thực hành code giao diện form số 2 phần 1.
- Thực hành code giao diện form số 2 phần 2.
- Thực hành code giao diện form số 2 phần 3.
- Tìm hiểu các thẻ về bảng.
- Hướng dẫn code giao diện bảng số 1.
- Hướng dẫn code giao diện bảng số 2.
- Hướng dẫn làm responsive cho bảng.

## Chương 7: Các kiến thức bổ sung:

- Review lại toàn bộ kiến thức đã học.
- Những lưu ý, cập nhật và cách luyện tập.
- Chia sẻ các từ tiếng Anh hay gặp khi đặt tên với BEM
- Các thẻ HTML hay gặp khác.
- Làm sao để cải thiện con mắt thẩm mỹ.
- Một số kênh youtube hay về HTML, CSS
- Một số tài khoản Instagram hay mà các bạn nên theo dõi.
- Các extensions bổ ích mà bạn nên dùng
- Chia sẻ kinh nghiệm làm sao code tốt hơn.
- Các thuật ngữ trong ngành web mà bạn nên biết
- Codepen là gì ? và vì sao bạn nên biết.
- Các kỹ năng khác nên có của một developer.
- Tìm hiểu thêm vài kiến thức về CSS khác.
- Làm sao để tùy biến giao diện cho wordpress với CSS
- Lời cảm ơn chân thành.
- Vẫn chưa hết! Khóa học cắt giao diện nâng cao từ A-Z
