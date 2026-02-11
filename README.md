# **cherry-pick**
- [有衝突的 cherry-pick](#有衝突的-cherry-pick)

## **有衝突的 cherry-pick**
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- **git cherry-pick <commit 的 hash 值(7 碼)> <commit 的 hash 值(7 碼)> ...**，發生衝突
    - 複製指定的 commit 到 HEAD 指向的 commit 後面。
- 解決衝突
    - 在本地端手動解決衝突，並刪除 Git 的衝突標記。
    - Git 的衝突標記：「<<<<<<<」、「=======」、「>>>>>>>」。
- **git add <檔案名稱.副檔名>**
    - 將檔案標記為衝突已解決。
- **git cherry-pick --continue**
    - 繼續執行 cherry-pick。
- **git push -u <遠端名稱(origin)> <分支名稱>**