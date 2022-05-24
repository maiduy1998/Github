see file https://shareprogramming.net/tong-hop-35-lenh-git-co-ban/#git_checkout
### Comments git 
# Thao tác với file 
   * mkdir Tạo thư mục 
   * git rm -r--cached namefile
# git init 
    Tạo một kho chứa Git
# git clone
    Sao chép một kho chứa đã tồn tại

### Cập nhật thay đổi

# git add .
    Sau khi bạn thay đổi source code: thêm mới, sửa, xoá files,… Bạn cần phải cập nhật lên Staging Area. Để cập nhật hết các files:
# git commit -m ""
    Sau lệnh add, bạn cần sử dụng câu lệnh Commit để đây thông tin thay đổi lên Local Respository:
  * git commit --amend -m "update last , . gitignore" Lệnh ko tạo thêm commit chỉ thêm 1 file update .gitignore mới.
# git push
    Cập nhật thay đổi từ phía client
  * git push origin [branch name] (thiết lập đúng branch muốn gửi file lên respository)
  * git push origin --delete [branch name] (xóa nhánh từ xa)
# git pull 
    Cập nhật thay đổi ở trên github
# git restore
    Phục hồi những file đã xóa

# git log-Xem lại lịch sử commit
    Lệnh git log sẽ cho bạn biết về người commit, ngày giờ, message của những lần commit đó.
  * git log --oneline (hiển thị lịch sử commit trên 1 line)
  * git log --oneline --graph (hiển thị lịch sử bằng graph)
# git status
    Cho biết trạng thái thay đổi 

## Xem thay đổi trước khi push

# git diff
Lệnh này giúp bạn biết những gì đã được thay đổi giữa nhánh hiện tại và nhánh trước nó.
  * systax:git diff Mã head mã head ex:git diff 33a8b2c 3b649b3--stat=> tìm sự thay đổi của các commit
## Lệnh về branch

# git branch
    Hiển thị branch có trên local
  * git checkout/git switch  branchname
  * git branch namebranch
# git remote git remote add origin https://github.com/maiduy1998/Github.git
    lệnh để tạo kết nối giữa local và repo
  * git remote => để liệt kê các liên kết sử dụng lệnh
  * git remote -v => Hiện thị thông tin chi tiết hơn, có thêm đường dẫn đến remote Repo
  * git remote show origin => xem remote origin