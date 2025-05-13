# **測試**
- [將檔案 push 到 GitHub 上](#將檔案-push-到-GitHub-上)
- [將檔案 push 到 GitHub 上的指定資料夾內](#將檔案-push-到-GitHub-上的指定資料夾內)
- [衝突](#衝突)

## **將檔案 push 到 GitHub 上**
- [第一次 push](#第一次-push)
- [其他 push](#其他-push)
### **第一次 push**
- **git remote add 遠端名稱( origin ) 複製網址**
	- 與遠端儲存庫連結
- **echo "# 標題" >> README.md**
	- 建立一個 README.md 檔，內容有一個標題	
- **git add 檔案名稱.副檔名**
	- 將檔案加入暫存區
- **git commit -m "版本訊息"**
	- 提交到儲存庫
- **git push -u 遠端名稱( origin ) 分支名稱( master )**
	- 將本地端的檔案推到遠端儲存庫，並建立追蹤關係
	- 登入：Sign in with your browser
	- 授權：Authorize git-ecosystem
	- push 成功：Authentication Succeeded	
### **其他 push**
- **git add 檔案名稱.副檔名**
- **git commit -m "版本訊息"**
- **git push 遠端名稱( origin ) 分支名稱( master )**

## **將檔案 push 到 GitHub 上的指定資料夾內**
- [在 GitHub 上建立資料夾](#在-GitHub-上建立資料夾)
- [在本地端建立資料夾](#在本地端建立資料夾)
### **在 GitHub 上建立資料夾**
- 資料夾：image_1
- 建立資料夾
	- Add file -> Create new file -> 在網址後輸入「名稱/」變成資料夾 -> 輸入檔案名稱 -> Commit changes -> 輸入 commit 內容 -> 選擇 Commit directly to the master branch -> Commit changes
- **git pull 遠端名稱( origin ) 分支名稱( master )** 
	- 與遠端儲存庫同步資料
- 將檔案放入 pull 下來的資料夾內
- **git add 資料夾名稱/檔案名稱.副檔名**
- **git commit**
- **git push**
### **在本地端建立資料夾**
- 資料夾：image_2
- 在與遠端儲存庫連結的本地端資料夾內，建立一個資料夾
- 將檔案放入新建立的資料夾內
- **git add 資料夾名稱/檔案名稱.副檔名**
- **git commit**
- **git push**

## **衝突**
- [本地端的不同分支合併衝突](#本地端的不同分支合併衝突)
### **本地端的不同分支合併衝突**
- 在 master 分支上
	- 新增檔案 -> git add -> git commit
- **git branch 分支名稱**
	- 建立分支
- **git checkout 分支名稱**
	- 切換分支
- 在 conflict-practice 分支上
	- 修改檔案 -> git add -> git commit
- 在 master 分支上
	- 修改檔案 -> git add -> git commit
- **git merge --no-commit 分支名稱**
	- 將分支名稱( conflict-practice )合併到 HEAD 指向的分支( master )，並且不自動產生 commit
- 發生衝突
	- 本地端的兩個分支版本不一樣
- 解決衝突
	- 在本地端手動解決衝突，並刪除 Git 的衝突標記
	- Git的衝突標記：「<<<<<<<」、「=======」、「>>>>>>>」
- **git add**
- **git commit**
	- 解決衝突，merge 本地端的兩個分支