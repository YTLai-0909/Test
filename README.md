# **cherry-pick**
- [沒有衝突的 cherry-pick](#沒有衝突的-cherry-pick)

## **沒有衝突的 cherry-pick**
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- **git cherry-pick <commit 的 hash 值(7 碼)> <commit 的 hash 值(7 碼)> ...**
    - 複製指定的 commit 到 HEAD 指向的 commit 後面。
- **git push -u <遠端名稱(origin)> <分支名稱>**