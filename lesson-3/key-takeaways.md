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