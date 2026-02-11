# **revert**
- [沒有衝突的 revert](#沒有衝突的-revert)

## **沒有衝突的 revert**
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- 在 revert-no-conflict 分支上
    - 新增檔案 → git add → git commit
    - 編輯檔案 → git add → git commit (多次)
- **git revert --no-commit <commit 的 hash 值(7 碼)>**
    - 將指定 commit 做反向。
    - --no-commit：不自動產生 commit。
- **git commit**
    - 撰寫 revert 的 commit 內容。
- **git push -u <遠端名稱(origin)> <分支名稱>**