# **將檔案 push 到 GitHub 上**
- [基本設定](#基本設定)
- [第一次 push](#第一次-push)
- [其他 push](#其他-push)

## **基本設定**
- **git config --global user.name <"名字">**
    - 設定姓名。
- **git config --global user.email <信箱>**
    - 設定信箱。
- **git init**
    - 在本地端資料夾建立 Git 儲存庫。

## **第一次 push**
- **git remote add <遠端名稱(origin)> <複製網址>**
    - 建立本地端與遠端儲存庫的連結。
- 新增並編輯檔案
- **git add <檔案名稱.副檔名>**
    - 將檔案加入暫存區。
- **git commit**
    - 提交到儲存庫。
    - 進入預設編輯器：vim。
    - i：進入編輯模式。
    - Esc：退出編輯模式。
    - :wq：保存並退出。
- **git push -u <遠端名稱(origin)> <分支名稱>**
    - 將本地端的檔案推到遠端儲存庫，並建立本地端的分支與本地端的遠端追蹤分支的追蹤關係。
    - 登入：Sign in with your browser。
    - 授權：Authorize git-ecosystem。
    - push 成功：Authentication Succeeded。

## **其他 push**
- 新增並編輯檔案
- **git add <檔案名稱.副檔名>**
- **git commit**
- **git push <遠端名稱(origin)> <分支名稱>**