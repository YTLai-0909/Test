# **將檔案 push 到 GitHub 上的指定資料夾內**
- [在 GitHub 上建立資料夾](#在-github-上建立資料夾)

## **在 GitHub 上建立資料夾**
- 在 GitHub 上建立分支
    - 在 master 上切新分支。
    - 點選 master 分支 → 按下 Commits → 點選想要的 commit → 按下右上角的 Browse files → 點選分支的下拉選單 → 在搜尋框輸入分支名稱 → 出現提示「Create branch <分支名稱> from <commit 的 hash 值(7 碼)>」 → 按下提示建立分支。
- 在新分支上建立資料夾並 commit
    - 確保分支選單是新分支 → Add file → Create new file → 在網址後輸入「資料夾名稱/」 → 輸入「檔案名稱.副檔名」 → 輸入檔案內容 → Commit changes → 輸入 commit 訊息 → 選擇 Commit directly to the <分支名稱> branch → Commit changes。
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- **git pull <遠端名稱(origin)> <分支名稱>**
    - 抓取遠端指定分支的最新版本，並更新本地端對應的分支。
- 在本地端將檔案放入 GitHub 上建立的資料夾內
- **git add <資料夾名稱/檔案名稱.副檔名>**
- **git commit**
- **git push -u <遠端名稱(origin)> <分支名稱>**