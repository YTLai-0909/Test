# **rebase -i**
- [reorder 重新排序 commit](#reorder-重新排序-commit)

## **reorder 重新排序 commit**
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- 在 rebase-i-reorder 分支上
    - 新增檔案 → git add → git commit
    - 編輯檔案 → git add → git commit (多次)
- **git rebase -i HEAD~3**
    - 開啟互動式編輯器(Vim)。
    - 3：列出從 HEAD 開始往前的 3 筆 commit，包含 HEAD。
- 手動調整 commit 的順序
    - dd：剪下。
    - P：貼上，貼在游標所在的列的上面。
    - p：貼上，貼在游標所在的列的下面。 
    - :wq：保存並退出。
- **git push -u <遠端名稱(origin)> <分支名稱>**