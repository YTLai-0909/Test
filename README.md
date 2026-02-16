# **rebase -i**
- [edit 修改 commit 的內容與訊息](#edit-修改-commit-的內容與訊息)

## **edit 修改 commit 的內容與訊息**
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- 在 rebase-i-edit 分支上
    - 新增檔案 → git add → git commit
    - 編輯檔案 → git add → git commit (多次)
- **git rebase -i HEAD~3**
    - 開啟互動式編輯器(Vim)。
    - 3：列出從 HEAD 開始往前的 3 筆 commit，包含 HEAD。
- 將 commit 前面的 pick 改成 edit，並儲存
    - i：進入編輯模式。
    - Esc：退出編輯模式。
    - :wq：保存並退出。
- Git 暫停在指定的 commit，編輯 commit 內容
- **git add <檔案名稱.副檔名>**
    - 將檔案加入暫存區。
- **git commit --amend**
    - 開啟互動式編輯器(Vim)，編輯 commit 訊息。
- **git rebase --continue**
    - 繼續執行 rebase。
- **git push -u <遠端名稱(origin)> <分支名稱>**