# **tag**
- [Annotated Tag (有附註的 tag)](#annotated-tag-有附註的-tag)

## **Annotated Tag (有附註的 tag)**
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- 在 annotated-tag 分支上
    - 新增並編輯檔案 → git add → git commit (多次)
- **git tag -a annotated-1.0.0 <commit 的 hash 值(7 碼)>**
    - 創建 tag。
    - annotated_tag.txt 的第一版。
- 開啟互動式編輯器(Vim)，編輯 tag 訊息
    - i：進入編輯模式。
    - Esc：退出編輯模式。
    - :wq：保存並退出。
- **git tag -a annotated-1.1.0 <commit 的 hash 值(7 碼)>**
    - 在 annotated_tag.txt 裡新增內容。
- 開啟互動式編輯器(Vim)，編輯 tag 訊息
- **git tag -a annotated-1.1.1 <commit 的 hash 值(7 碼)>**
    - 在 annotated_tag.txt 裡修改內容。
- 開啟互動式編輯器(Vim)，編輯 tag 訊息
- **git tag -a annotated-2.0.0 <commit 的 hash 值(7 碼)>**
    - annotated_tag.txt 的第二版。
- 開啟互動式編輯器(Vim)，編輯 tag 訊息
- **git push -u <遠端名稱(origin)> <分支名稱>**
- **git push <遠端名稱(origin)> --tags**
    - push 所有的 tag 到遠端。