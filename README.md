## Lệnh git cơ bản

`git init` : khởi tạo git

`git add .`

`git commit -m"<msg>"`

`git log --oneline` : để xem lịch sử commit

`git remote add <remote_name> <url>` : tạo remote tới repo github

`git pull <remote_name> main` : pull nhánh main về local, lệnh này bao gồm git fetch và merge

`git checkout -b <branch_name>` : vừa tạo branch vừa chuyển branch.

`git checkout <commit_code>` : để quay lại commit có mã <commit_code>

`git checkout <branch_name>` : để chuyển nhánh của mình và code


`git push <remote_name> <branch_name>` : 
- Khi push lần đầu, đồng nghĩa với việc tạo thêm một nhánh <branch_name> ở trên github và
- Đẩy nhánh <branch_name> ở local lên nhánh <branch_name> ở github


## Quy trình chung đối với mọi người: 
**VD: có một remote tên an_remote**
- Đầu tiên pull nhánh main trên git về mà code: git pull an_remote main
- Không thao tác trên nhánh MAIN/MASTER ở GITHUB
- Pull về rồi tạo một branch với tên của mình vd : git checkout -b nguyenvanan
- Khi làm code xong => dùng git push an_remote nguyenvanan
- Lên github => chọn nhánh nguyenvanan => nhấp cái link xanh blue có chữ "1 commit ahead" => Button "Create pull request"
- Ghi title, desc ở ô write rõ ràng => Create pull request
- Nhắn lên nhóm hoặc nhắn trước khi push lên cũng đc
- Còn lại để thằng quản lý git xử lý, bấm nhiều quá hư project

## Lưu ý:
- <remote_name>/<branch_name> : là trỏ đến nhánh <branch_name> trên github mà <remote_name> trỏ đến
- Luôn kiểm tra có đang ở **nhánh của mình không**? nếu không thì chuyển về nhánh của mình rồi code

## Đối với người quản lý git:
- Một khi có merge thì **thông báo lại cho nhóm**
- Nếu có đụng độ trên main khi merge các nhánh từ thành viên thì **thành viên đó sẽ hỗ trợ giải quyết**
