# **revert**
- [有衝突的 revert](#有衝突的-revert)

## **有衝突的 revert**
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- 在 revert-conflict 分支上
    - 新增並編輯檔案 → git add → git commit (多次)
- **git revert --no-commit <commit 的 hash 值(7 碼)>**，發生衝突
    - 將指定 commit 做反向。
    - --no-commit：不自動產生 commit。
- 解決衝突
    - 在本地端手動解決衝突，並刪除 Git 的衝突標記。
    - Git 的衝突標記：「<<<<<<<」、「=======」、「>>>>>>>」。
- **git add <檔案名稱.副檔名>**
    - 將檔案標記為衝突已解決。
- **git commit**
    - 解決衝突，撰寫 revert 的 commit 內容。
- **git push -u <遠端名稱(origin)> <分支名稱>**