# 📘 Git-Learning-Note

## 📑 Table of Contents
- [🆕 Create a new repository](#-or-create-a-new-repository-on-the-command-line)
- [📤 Push an existing repository](#-or-push-an-existing-repository-from-the-command-line)
- [🗑️ Remove unnecessary files](#️-remove-the-file-that-we-dont-need-to-add-when-push)
- [🐍 Python](#-python)
- [🎬 Tải Video yt-dlp](#-tải-video-yt-dlp)


````markdown
# 🚀 Hướng dẫn khởi tạo Project với Git & GitHub

Tài liệu này hướng dẫn cách khởi tạo và đẩy (push) project từ máy local lên GitHub, áp dụng cho cả hai trường hợp:  
1️⃣ Bắt đầu từ **project có sẵn trong máy**  
2️⃣ Bắt đầu từ **repo GitHub có sẵn**

---

## 💡 Trường hợp 1: Bắt đầu từ Local Project

> Khi bạn đã có sẵn project trong máy và muốn đưa lên GitHub.

### Các bước thực hiện:

```bash
# 1. Mở terminal trong thư mục project
git init

# 2. Thêm toàn bộ file vào vùng staging
git add .

# 3. Tạo commit đầu tiên
git commit -m "Initial commit"

# 4. Tạo repository trống trên GitHub (ví dụ: myproject)
#    rồi kết nối local repo với GitHub repo
git remote add origin https://github.com/username/myproject.git

# 5. Đặt nhánh chính là main
git branch -M main

# 6. Đẩy code lên GitHub
git push -u origin main
````

✅ **Kết quả:** Project local của bạn đã được đẩy lên GitHub thành công.

---

## 💡 Trường hợp 2: Bắt đầu từ Repo GitHub

> Khi bạn tạo repo trước trên GitHub và muốn clone về để làm việc.

### Các bước thực hiện:

```bash
# 1. Clone repo từ GitHub về máy
git clone https://github.com/username/myproject.git

# 2. Di chuyển vào thư mục project
cd myproject

# 3. Thực hiện code, thêm file mới...

# 4. Thêm và commit thay đổi
git add .
git commit -m "First commit"

# 5. Đẩy code lên GitHub
git push
```

✅ **Kết quả:** Code mới được cập nhật lên GitHub.

---

## 📘 Tóm tắt nhanh

| Tình huống      | Bắt đầu từ Local Project             | Bắt đầu từ GitHub Repo       |
| --------------- | ------------------------------------ | ---------------------------- |
| Khi nào dùng    | Có sẵn code trong máy                | Làm việc với repo có sẵn     |
| Bước đầu tiên   | `git init`                           | `git clone`                  |
| Thứ tự thao tác | Commit local → Kết nối GitHub → Push | Clone → Code → Commit → Push |

---

## 💬 Gợi ý

* Dùng `git status` để kiểm tra trạng thái file.
* Dùng `git log` để xem lịch sử commit.
* Dùng `git pull` để cập nhật thay đổi mới nhất từ GitHub.
* Dùng `.gitignore` để loại bỏ file không cần theo dõi (VD: venv, node_modules, .DS_Store, ...).

---

✳️ **Tips:** Nếu đây là lần đầu bạn đẩy code lên GitHub, đảm bảo bạn đã đăng nhập Git bằng token hoặc SSH key.

```

---

Bạn muốn tôi thêm phần **hướng dẫn tạo `.gitignore`** chuẩn cho Python (hoặc Web project) vào cuối README luôn không?
```


## 🆕 …or create a new repository on the command line

1.  echo "# Learning-Airflow-Begining" >> README.md  
2.  git init  
3.  git add README.md  
4.  git commit -m "first commit"  
5.  git branch -M main  
6.  git remote add origin https://github.com/MonkeyNerdCoding/Learning-Airflow-Begining.git  
7.  git push -u origin main  

---

## 📤 …or push an existing repository from the command line

1. git config --global user.name "MonkeyNerdCoding"
2. git config --global user.email "sockhi2004@gmail.com"
   
1.  git remote add origin https://github.com/MonkeyNerdCoding/Learning-Airflow-Begining.git  
2.  git branch -M main  
3.  git push -u origin main  

---

## After push 
1. git add .
2. git commit -m ""
3. git push

---

## Merge and Pull
### 1. Merge (giữ lịch sử merge):
```bash
git pull --no-rebase origin main
````

### 2\. Rebase (lịch sử thẳng, commit của bạn sẽ nằm trên commit mới nhất của remote):

```bash
git pull --rebase origin main
```

Sau khi `pull` thành công (dù `merge` hay `rebase`), bạn chỉ cần:

```bash
git push -u origin main
```

```
Bạn có thể giữ nguyên nội dung mặc định (hoặc chỉnh lại nếu muốn).
Nhấn Ctrl + O (Write Out) để lưu file.
Nhấn Enter để xác nhận tên file.
Nhấn Ctrl + X để thoát nano.

```

---

## 🗑️ Remove the file that we don't need to add when push 

1. ♻️ git reset venv  

---

## 🐍 Python 

1.  python -m .venv venv  
2.  ./.venv/Scripts/Activate.ps1  

---

## 🎬 Tải Video yt-dlp

- 📌 link github : https://github.com/yt-dlp/yt-dlp?tab=readme-ov-file#installation  
- 🌍 Link check xem các nền tảng hỗ trợ : https://github.com/yt-dlp/yt-dlp/blob/master/supportedsites.md##  
- 📖 link bài viết hướng dẫn : https://blogchiasekienthuc.com/thu-thuat-internet/cach-su-dung-yt-dlp-de-tai-video.html  
- 🎥 link video hướng dẫn https://www.youtube.com/watch?v=TrDPEpbdZIE  

### 🔽 Các bước:
1. ⬇️ Tải qua cmd hoặc powershell  
2. ▶️ lệnh chạy `./yt-dlp.exe [Link-video-muốn-tải]` (có thể bỏ `./` ở phía trước nếu không được)  
3. 📝 Lệnh tải video + phụ đề dạng `.srt`:  

```bash
yt-dlp --write-subs --sub-format srt --sub-lang en,vi --convert-subs srt -f mp4 <link_video>

👉 Trong đó:
--write-subs → tải phụ đề.
--sub-format srt → định dạng SRT.
--sub-lang en,vi → tải phụ đề tiếng Anh + tiếng Việt (có thể thay theo ngôn ngữ bạn muốn).
--convert-subs srt → chuyển phụ đề về dạng .srt.
-f mp4 → tải video định dạng mp4.

```

🔎 Lệnh check xem video đó có sub nào
```bash
yt-dlp --list-subs

```
👉 Nếu nó thể hiện no sub thì dùng lệnh bên dưới:
```bash
yt-dlp --write-auto-subs --sub-lang en --sub-format srt --convert-subs srt -f mp4 https://www.youtube.com/watch?v=vMgFadPxOLk


