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

- Sử dụng một số trang có UI theo mẫu trước: https://collectui.com/
- Modifiers sẽ luôn đi kèm với block hoặc elements đó khi mà đang sử dụng.

9. Bài tập chương 1

# Tạo 1 file HTML như đã học và làm tât cả các bài dưới đây vào.

1. Liệt kê 10 thẻ inline, 10 thẻ block và các thẻ semantic HTML5 mà bạn biết

2. Làm 1 ví dụ về BEM cho block có tên là `boy`

3. Hãy làm 1 ví dụ về sự kết hợp giữa thẻ block và thẻ inline

4. Áp dụng kiến thức về BEM đặt tên cho UI này: static.collectui.com/shots/1436570/dropdown-menu-large Hint: Block có tên `dropdown`

5. Giới thiệu bài tập chương 1 phần 1:

6. Nắm vững Emmet cơ bản trong VSCode:

- Emmet giúp code tốt hơn và nhanh hơn.
- Sử dụng phím 'Alt và mũi tên lên xuống' để di chuyển 1 đoạn code.
- Tạo 1 dòng y chang nhau: Shift + Alt + mũi tên lên xuống
- ul>li\*10{item$}
- Tạo thẻ cùng cấp với nhau: h1.title+p.desc+div.demo>p.text
  h1.title+p.desc+.demo>p.text+p.text2^.job
- Có thể vô google gõ: emmet cheat sheet

## Chương 2: Kiến thức CSS cơ bản phần 1

1. CSS reset là gì ? Tại sao phải dùng reset CSS ?

- Lấy những reset css là sẽ lấy trong đây:
  https://meyerweb.com/eric/tools/css/reset/

2. Cấu trúc của 1 đoạn code trong CSS như thế nào ?

selector {
property: value;
}

Selector:
Tags: p, div, h1, main, a, span
Class: .demo, .header, .boy
Id: #container, #footer

Property: color, background-color
Value: red, orange, yellow

3. Tìm hiểu thuộc tính color, các giá trị về màu sắc cần nắm vững.

- color: value

  named: red, orange, blue, green
  hexa: #ffa400, #666666 -> #666, #7cd7cd -> #7cd
  rgb: rgb(0,0,0), rgb(255,255,255)
  rgba: (alpha: opacity 0 -> 1) rgba(0,0,0,0.5)

4. Nắm vững kiến thức về kích thước trong CSS:

- khi bị nó tràn ra ngoài, tràn khỏi kích thước của mình nên mình muốn ẩn đi thì dùng : overflow: hidden.
- Sử dụng các thuộc tính về kích thước như là:
  min-width, max-width, min-height, max-height.

5. Làm hình nền với thuộc tính về background:

- Các thuộc tính thêm về background như là:
  background-color, background-size, background-attachment
  background-position, background-repeat

6. Các đơn vị trong css nên biết.

- có 2 đơn vị là % và vw,vh.
  % thì nó ăn theo độ dài, độ rộng của div cha chưa nó.
  vw,vh nó chỉ quan tâm mỗi viewport(màn hình) mà nó hiển thị mà thôi.

7. Đơn vị em và rem khác nhau như thế nào ?

- mặc định font-size trình duyệt là 100% -> 16px
- 1em = 1rem = 16px

Phân biệt em với rem:

- em là đơn vị sẽ phụ thuộc vào thuộc tính font-size của chính nó hoặc phần tử chứa nó.
- rem Là đơn vị sẽ phụ thuộc vào thuộc tính font-size của thẻ html của nó
  Do 100% là 12px, nó quá là lẻ và khó quy đổi
  nên là ta quy ước luôn là
  html {
  font-size: 62.5%;
  1rem = 10px
  }

8. Thuộc tính về border cơ bản:

- border: border-width border-style border-color
- border-raius: chỉ số.
  (border-top, border-right, border-left, border-bottom)
  (border-top-left, border-top-right, border-bottom-left, border-bottom-right)
- Điểm khác nhau giữa thằng outline và border là outline sẽ không thể có được bo góc.

9. Nắm rõ thuộc tính margin:

1 giá trị -> top = right = left = bottom = 20px
margin: 20px;

2 giá trị -> top = bottom = 20px, right = left = 40px
margin: 20px 40px;

3 giá trị -> top = 10px, right = left = 20px, bottom = 30px
margin: 10px 20px 30px;

4 giá trị -> top = 10px, right = 20px, bottom = 30px, left 40px
margin: 10px 20px 30px 40px;

Đối với thẻ block mà muốn căn giữa thì có 2 thuộc tính này.
margin-left sẽ cho block đó nằm sát vào bên phải.
margin-left: auto;
margin-right: auto;

- Khi làm với margin sẽ có khái niệm margin collapse
  thì thằng margin sẽ lấy giá trị lớn hơn.

10. Hiểu về thuộc tính padding:

- margin (outer spacing) >< padding (inner spacing)
- các thông số của padding cũng y hệt như với là margin
  4 giá trị, 3 giá trị, 2 giá trị, 1 giá trị.

- Thuộc tính margin có thể sử dụng được số âm, còn padding thì KHÔNG ĐƯỢC DÙNG SỐ ÂM.

11. Tìm hiểu về box-sizing trong CSS:

Giá trị mặc định của box-sizing
box-sizing: content-box;
Ta cần chuyển nó thành:
box-sizing: border-box;

    content-box:
        width = width + padding-left + padding-right + border-left + border-right
        height = height + padding-top + padding-bottom + border-top + border-bottom

    border-box:
        width thực tế = width ban đầu - padding-left - padding-right - border-left - border-right
        height thực tế = height ban đầu - padding-top - padding-bottom - border-top - border-bottom

12. Tìm hiểu thuộc tính display:

- Có thể chuyển đổi từ thẻ inline sang thẻ block thì ta sẽ sử dụng là display: block hoặc inline-block
  Còn muốn ẩn luôn thẻ đó đi thì sử dụng display: none.

13. Các thuộc tính liên quan tới font cơ bản:

- Tìm kiếm : Google fonts
  https://fonts.google.com/
- Tăng kích cỡ: font-size
- In đậm lên : font-weight.
- Kiểu chữ: font-style

14. Các thuộc tính liên quan tới chữ bạn cần biết:

- line-height
  mặc định line height sẽ là 1.
  line-height: 1.5;

  text-align: left;
  text-align: center;
  text-align: justify;

  Letter spacing chính là khoảng cách giứa các chữ. Mặc định letter spacing là 0px
  letter-spacing: 1px;

  word-spacing chính là khoảng cách giữa các từ
  word-spacing: 5px;

  Hiển thị dấu 3 chấm trên 1 hàng
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;

  Hiển thị dấu 3 chấm tới hàng thứ 3
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-line-clamp: 3;
  overflow: hidden;
  text-overflow: ellipsis;

  dùng để cho chữ nó tự động rớt xuống hàng cho vừa độ rộng
  word-break: break-all;

15. Tìm hiểu thuộc tính cho hình ảnh:

- Đối với hình ảnh thì thẻ img là thẻ inline nên là nếu muốn ra giữa thì sử dụng thuộc tính text-align:center
- còn nếu ko thì chuyển nó về block sau đó sử dụng thuộc tính : margin: 0 auto là sẽ căn giữa đc.
- Muốn ảnh hiển thị đủ trong khung của mình muốn thì có thuộc tính: object-fit: cover

16. Pseudo là gì ? Các pseudo cơ bản người mới học nên biết:

- Có các trạng thái như là: hover, visited,...

17. Bài tập chương 2 phần 1
18. Bài tập chương 2 phần 2

## Chương 3: Kiến thức CSS cơ bản phần 2

1. Cách làm hình nền gradient, chữ gradient trong CSS:

- gradient đc hiểu là các màu được mix lại với nhau.
- thường sẽ dùng gradient khi có background-image:
  vị trí: to right, to left, to bottom, to top.
  to right bottom, to left bottom, to left top, to right top.
  bo góc: 120deg
  màu: color1
  color2

- Muốn làm chữ trong suốt thì thuộc tính color: transparent và thêm 2 thuộc tính nữa:
  -webkit-background-clip: text;
  background-clip: text;

2. Hiển thị 2 hình nền với background-image:

- kết hợp lớp gradient với image.
  background-image: gradient , image

3. Caniuse là gì ? và tại sao bạn nên biết:

- trang web caniuse xem các thuộc tính khác nhau sẽ có hỗ trợ ở trình duyệt khác nhau hay ko ?
  VD: thuộc tính color có hỗ trợ bên trình duyệt IE hay ko ..
- Sử dụng rule @supports để có thể hiển thị tùy chỉnh.
  @supports(-webkit-background-clip: text){
  .title {
  }
  }

4. Sự khác nhau giữa 3 thuộc tính opacity, display, visibility:

- Opacity vẫn chiếm diện tích, có thể nhấn vào được
  opacity: 0.5;

  Visibility vẫn chiến diện tích, nhưng KHÔNG nhấn vào được
  visibility: hidden;

  display: none thì biến mất, ko chiếm diện tích, KHÔNG NHẤN VÔ ĐƯỢC.
  display: none;

5. Tìm hiểu về shadow trong CSS:

- shadow dùng để tạo độ bóng cho chữ.
  box-shadow: x y blur scale color
  giá trị của x y blur scale có thể là px

  inset là tạo độ bóng bên trong, outset (giá trị mặc định) là tạo độ bóng bên ngoài

- Làm tương tự với text.

6. Sử dụng biến trong CSS như thế nào ?

- khai báo trong thuộc tính root.
  :root {
  --tenbien:abcxyz;
  }

- khi muốn sử dụng thì phải sử dụng var(tên biến)

7. Hiểu rõ về độ ưu tiên trong CSS, xác định độ ưu tiên trong CSS đơn giản với VSCode:

- Tags < Class < id < inline < thuộc tính !important

x, y, z -> tags, class or atr, id.
VD: 0,0,1
0,1,0
1,0,0

8. Nắm vững kiến thức về child selectors:

- :first-child, :last-child.
- :nth-child(1,2,3,....): sẽ bắt đầu thứ tự từ 1.
- :nth-last-child...
- :not(...)
- :nth-child(odd), :nth-child(even)

9. Nắm vững kiến thức về type selectors:

- type thì nó sẽ check theo kiểu, theo Tags
- Còn child sẽ check thì vị trí.

có thể sử dụng : first-of-type, last-of-type, nth-of-type.
nth-last-of-type

10. Thành thạo combinators trong CSS:

- CSS combinators sẽ có 2 cái là dấu + và ~.

dấu + hay dấu ~ thì luôn luôn phải cùng cấp với nhau thì mình mới css được.
và tất nhiên khi css thì phải css từ trên xuống dưới.
VD: h2 ~ .abc

11. Tìm hiểu thêm các selectors nâng cao:

- Css cho các attr
  VD: css cho các thẻ a có thuôc tính attr là https
  a[href^="https"]{
  color: blue;
  }
  kết thúc thì sử dụng dấu '$'
  có chứa thì sử dụng dấu '\*'

- Có trang web sẽ chia sẻ vấn đề css nâng cao.
  https://www.w3schools.com/cssref/css_selectors.asp

12. Nắm vững thuộc tính transition cơ bản:

- transition dùng để làm hiệu ứng, dùng để ẩn/hiện một cái nào đấy.
  transition: property timer(2s) linear
  có transition-delay để delay ẩn/hiển sau 1 khoảng thời gian.

13. Bài tập chương 3.

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
