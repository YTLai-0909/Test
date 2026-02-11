# **rebase -i**
- [reword 單筆和多筆 commit](#reword-單筆和多筆-commit)

## **reword 單筆和多筆 commit**
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- 在 rebase-i-reword 分支上
    - 新增並編輯檔案 → git add → git commit (多次)
- **git rebase -i <commit 的 hash 值(7 碼)>^**
    - 開啟互動式編輯器(Vim)。
    - ^：目前 commit 的前一個 commit。
    - rebase -i 會從指定 commit 的下一個 commit 開始列出，直到 HEAD 指向的 commit。
- 將 commit 前面的 pick 改成 reword，並儲存
    - reword 單筆 commit。
    - i：進入編輯模式。
    - Esc：退出編輯模式。
    - :wq：保存並退出。
- 開啟編輯器(Vim)，編輯 commit 訊息
- **git rebase -i HEAD~3**
    - 開啟互動式編輯器(Vim)。
    - 3：列出從 HEAD 開始往前的 3 筆 commit，包含 HEAD。
- 將 commit 前面的 pick 改成 reword，並儲存
    - reword 多筆 commit。
- 開啟編輯器(Vim)，編輯 commit 訊息 (多次)
- **git push -u <遠端名稱(origin)> <分支名稱>**