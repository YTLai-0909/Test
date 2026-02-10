# **merge**
- [沒有衝突的 merge](#沒有衝突的-merge)

## **沒有衝突的 merge**
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立 merge-no-conflict 分支。
- **git checkout <分支名稱>**
    - 切換到 merge-no-conflict 分支。
- 在 merge-no-conflict 分支上
    - 新增檔案 → git add → git commit
- **git branch <分支名稱>**
    - 在 merge-no-conflict 上切新分支。
    - 建立 tmp-merge-no-conflict 分支。
- **git checkout <分支名稱>**
    - 切換到 tmp-merge-no-conflict 分支。
- 在 tmp-merge-no-conflict 分支上
    - 新增內容 → git add → git commit
- **git checkout <分支名稱>**
    - 切換到 merge-no-conflict 分支。
- 在 merge-no-conflict 分支上
    - 新增內容 → git add → git commit
- **git merge --no-ff --no-commit <分支名稱>**
    - 將分支名稱(tmp-merge-no-conflict)合併到 HEAD 指向的分支(merge-no-conflict)。
    - --no-ff：不使用 Fast-forward 合併。
    - --no-commit：不自動產生 commit。
- **git commit**
    - 撰寫 merge 的 commit 內容。
- **git push -u <遠端名稱(origin)> <分支名稱>**