# **tag**
- [Lightweight Tag (輕量的 tag)](#lightweight-tag-輕量的-tag)

## **Lightweight Tag (輕量的 tag)**
- **git branch <分支名稱>**
    - 在 master 上切新分支。
    - 建立分支。
- **git checkout <分支名稱>**
    - 切換分支。
- 在 lightweight-tag 分支上
    - 新增並編輯檔案 → git add → git commit (多次)
- **git tag lightweight-1.0.0 <commit 的 hash 值(7 碼)>**
    - 創建 tag。
    - lightweight_tag.txt 的第一版。
- **git tag lightweight-1.1.0 <commit 的 hash 值(7 碼)>**
    - 在 lightweight_tag.txt 裡新增內容。
- **git tag lightweight-1.1.1 <commit 的 hash 值(7 碼)>**
    - 在 lightweight_tag.txt 裡修改內容。
- **git tag lightweight-2.0.0 <commit 的 hash 值(7 碼)>**
    - lightweight_tag.txt 的第二版。
- **git push -u <遠端名稱(origin)> <分支名稱>**
- **git push <遠端名稱(origin)> --tags**
    - push 所有的 tag 到遠端。