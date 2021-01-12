//git init
//cmd check git status
//git add
//git commit : dong goi nhung git add thanh 1 object
get commit -m 'Add readme file'
-m: them mo ta

//git log: history of commited file
//git diff: xem thay doi cua nhung file da modified
//git show: xem trong box co gi 
git show 3728320hfdjkhfj2389

//working directory: file dang su dung
//staging area: nhung file mau xanh la nam trong staging area
//git repository: luu nhung thay doi cua commit

//git checkout: co the xoa 1 so file hoac dong lenh chua len staging
git checkout -- <filename>
//git reset: sua 1 file tu staging xuong working

//git branch
make a new branch and checkout: git checkout -b <branch> (branching)
ex: git checkout -b feature/dog-class
check the working branch: git checkout <branch>
//git merging
A <---- B
git checkout A
git merge B
master <---- feature/dog-class
//git branch -D <branch> (delete a branch)

//git reset --soft <to_commit_id> (SHA1ID)
in case want to turn back before commit (in staging area)
//git reset --mixed <to_commit_id>
in case want to turn back before in stage (in working directory)
//git reset --hard <to_commit_id>
in case want to delete commit before that

//git revert <commit_id> : quay lai trang thai cua chi commit do thoi

Khong muon commit 1 so file thi tao 1 file .gitignore

//luu tru thong tin dang nhap khi push 
cmd: git config --global credential.helper store : not encript
cmd: git config --global credential.helper "cache --timeout=18000"
