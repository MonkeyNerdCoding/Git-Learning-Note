# 📘 Git-Learning-Note

## 🆕 …or create a new repository on the command line

1. ✍️ echo "# Learning-Airflow-Begining" >> README.md  
2. 🗂️ git init  
3. 📂 git add README.md  
4. ✅ git commit -m "first commit"  
5. 🌿 git branch -M main  
6. 🔗 git remote add origin https://github.com/MonkeyNerdCoding/Learning-Airflow-Begining.git  
7. 🚀 git push -u origin main  

---

## 📤 …or push an existing repository from the command line

1. 🔗 git remote add origin https://github.com/MonkeyNerdCoding/Learning-Airflow-Begining.git  
2. 🌿 git branch -M main  
3. 🚀 git push -u origin main  

---

## 🗑️ Remove the file that we don't need to add when push 

1. ♻️ git reset venv  

---

## 🐍 Python 

1. ⚙️ python -m .venv venv  
2. ▶️ ./.venv/Scripts/Activate.ps1  

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


