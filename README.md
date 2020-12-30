# btree-js
Demo: **[BTree](https://github.com/duongnt58/b-tree)**

Javascript thực hiện cài đặt cấu trúc cây [B-tree](https://en.wikipedia.org/wiki/B-tree) từ 3 khóa trở lên.
 
Tại đây chúng ta có thế tìm kiếm hoặc thêm mới một note. Thuật toán thêm mới một note như sau:

1. Duyệt qua cây để tìm kiếm được đúng lá để chèn giá trị.
2. Chèn thêm một giá trị vào nút lá.
    * Nếu nút đang duyệt qua còn khoảng trống thì chèn giá trị vào nút đó.
    * Nếu nút đang duyệt đã đủ phần tử và nút đó là nút gốc thì tách nút và tạo nút cha mới.
    * Nếu nút đang duyệt đã đủ phần tử và đang là nút cha thì chia nút và chèn thêm phần tử vào nút cha. Duyệt lại nút cha và lặp lại cho đến khi các nút đủ phần tử.
3. Quay lại tất cả các đường và kết nối tất cả các nút tách với các nút cha mẹ thích hợp.

Via: [Allen Chang](https://allendevelops.wordpress.com) and [Eric Yang](http://www.eric-y.com).
