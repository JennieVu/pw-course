# Undo things in GIT
## Xem lịch sử commit: git log 
## Thay đổi commit message: git commit --amend
### Quy trình theo các bước
#### Cách 1: git commit -amend
- git log 
- Gõ q để quit
- Gõ git commit --amend 
- Gõ i để vào chế độ insert (ví dụ: gõ thêm feat:)
- Gõ esc để thoát 
- Gõ : wq (write and quit)
#### Cách 2: git commit --amend -m"message" (Thay đổi message của commit cuối cùng)
-  Ví dụ: git commit --amend -m"chore: remove the unused lines" 
## Đưa từ vùng staging về working directory:
- git restore --staged <file> hoặc git restore --staged <file>. là chuyển tất
- P/S: Cách để add file từ working directory tới staging 
  - git status
  - git add <tên file>
  - git add. : là add hết 
## Đưa vùng repository về staging: git reset HEAD~1
- P/S: Cách để commit cấu trúc alf git commit - m"<tên file>
- Cách làm: 
    - git log 
    - git reset HEAD~1
    - git status (để xem lại)
## Loại bỏ các file không cần git track: .gitignore <file>
- Điền thêm tiền tố .gitignore trước tên file hoặc  folder.
# Javascript
## Name convention:
- snake_case: file chưa dùng
- kebab-case: tên file 
- camalCase: tên biến 
- PascalCase: tên class
## Data type/Data structure: 
- Dữ liệu nguyên thuỷ (primitive types): string, number, boolean, null, undefined, symbol, bigint. 
 - Đặc điểm: 
   - Lưu trực tiếp gái trị vào biến
   - Kích thước dữ liệu nhỏ, cố định 
   - Tạo sự động lập khi gán sang biến khác
- Dữ liệu tham chiếu (reference types): obiejct, array, function, regex
   - Lưu địa chỉ đén vùng dữ liệu được lưu
   - Cấu trúc phức tạp, thay đổi kích thước
### Dấu nháy đơn và nháy kép:
- Công dụng: Chỉ chứa text tĩnh, không có biến. Đoạn text ngắn, nội dung ít thay đổi.
  - console.log("Toi la Phong");
  - console.log('Toi la Phong');
  - Nếu dùng 2 cái này thì sẽ nối chuỗi bằng dấu +
### Backticks (`): Trong Java được gội là template literals
#### Công dụng: 
- Thay vì phải nối chuỗi bằng toán tử +, bạn có thể viết thẳng biến hoặc biểu thức bên trong ${...}.
  - Ví dụ: let name = "Nga"; console.log('Tôi là ${name}`); 
- Viết nhiều dòng dễ dàng, không cần nối 
- Tích hợp biểu thức
### Object: 
- Nằm trong cặp ngoặc nhọn, có thuộc tính ở dạng key: value.
  - Key ở trong nháy ' hoặc ', ví dụ "name": Phong với key là name 
- Khai báo object: 
   - const student = { 
     - name: "Nam",
     - age: 20
    - };
- Thêm thuộc tính: Dùng dấu (.) Ví dụ: student.className ="12A1"; trong đó className là tên thuộc tính mới, "12A1" là giá trị
- Xoá thuộc tính: Dùng từ khoá delete. Format delete object.key;
  - Ví dụ delete student.age; => sau lệnh này student không còn age nữa.
- Lấy (truy cập) giá trị của một thuộc tính): 
  - Dùng dấu chấm: theo cú pháp object.key hoặc object["key"]
   - ví dụ: console.log(student.name); => In ra giá trị của "name"
### Array:
- Khai báo array: const fruits = ["Apple", "Banana", "Cherry"];
- Thêm phần tử
  - Cách 1: Thêm vào cuối bằng push(). Ví dụ: fruits.push("Orange");
  - Cách 2: Thêm vào đầu bằng unshift(). Ví dụ: fruits.unshift("Mango");
  - Gán trực tiếp qua chỉ số. Ví dụ fruits[fruits.length]= "grapes"; (cũng thêm vào cuối array)
- Xoá phần tử:
  - Xoá cuối bằng pop(). Ví dụ: const last = fruits.pop();
  - Xoá đầu bằng shift():. Ví dụ const first = fruits.shift();
  - Xoá ở tuỳ vị trí bằng splice(index,count):
- Truy xuất phần tử:
  - Dùng chỉ số index. Ví dụ console.log(fruits[0]);
### Function: 
- Khai báo hàm: function.tênhàm () {
     console.log("Xin chao, K12");
}
- Gọi hàm: tênhàm();
