# **衝突**
- [遠端與本地端的同分支合併衝突](#遠端與本地端的同分支合併衝突)

## **遠端與本地端的同分支合併衝突**
- 在 GitHub 上建立分支
    - 在遠端的 master 上切新分支。
    - 點選 master 分支 → 按下 Commits → 點選想要的 commit → 按下右上角的 Browse files → 點選分支的下拉選單 → 在搜尋框輸入分支名稱 → 出現提示「Create branch <分支名稱> from <commit 的 hash 值(7 碼)>」 → 按下提示建立分支。
- 在遠端 GitHub 的 same-branch-conflict 分支上
    - 確保分支選單是新分支 → Add file → Create new file → 在網址後輸入「檔案名稱.副檔名」 → 輸入檔案內容 → Commit changes → 輸入 commit 訊息 → 選擇 Commit directly to the <分支名稱> branch → Commit changes。
- **git branch <分支名稱>**
    - 在本地端的 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- 在本地端的 same-branch-conflict 分支上
    - 新增並編輯檔案 → git add → git commit
- **git push -u <遠端名稱(origin)> <分支名稱>**，push 失敗
    - Git 不允許在遠端版本比本地端版本新的情況下進行 push，避免覆蓋到他人的改動。
- **git pull <遠端名稱(origin)> <分支名稱>**，發生衝突
    - 遠端與本地端的分支版本不一樣。
- 解決衝突
    - 在本地端手動解決衝突，並刪除 Git 的衝突標記。
    - Git 的衝突標記：「<<<<<<<」、「=======」、「>>>>>>>」。
- **git add <檔案名稱.副檔名>**
    - 將檔案標記為衝突已解決。
- **git commit**
    - 解決衝突，merge 遠端與本地端的分支。
- **git push -u <遠端名稱(origin)> <分支名稱>**