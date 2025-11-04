# 🗂️ File Organizer

A **Python-based File Organizer** that automatically sorts files in a directory into categorized folders (like Images, Documents, Videos, Code, etc.) based on file extensions.  
It helps keep your workspace clean and well-structured with optional dry-run previews, undo functionality, and custom category configuration.

---

## 🚀 Features

- 📦 **Automatic Sorting:** Moves files into folders by type (Images, Documents, Audio, Videos, etc.)
- ⚙️ **Custom Categories:** Easily add or remove file type categories via interactive configuration.
- 🧪 **Dry Run Mode:** Preview what will happen before actually moving any files.
- ⏪ **Undo Last Operation:** Revert the last organization instantly.
- 🧹 **Clean Up:** Remove empty folders left after organizing.
- 🧾 **Logging:** Keeps a detailed log of all file movements and errors.
- 💾 **Config Persistence:** Saves your file type preferences in a JSON config file.

---

## 📁 Folder Structure

After organizing, your directory will look something like this:

```
📂 YourFolder/
 ┣ 📂 Images/
 ┃ ┣ photo1.jpg
 ┃ ┗ wallpaper.png
 ┣ 📂 Documents/
 ┃ ┣ resume.pdf
 ┃ ┗ notes.txt
 ┣ 📂 Videos/
 ┃ ┗ clip.mp4
 ┣ organizer_config.json
 ┣ organizer_log.txt
 ┗ file_organizer.py
```

---

## 🧰 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/file-organizer.git
cd file-organizer
```

### 2. Run with Python
Make sure you have **Python 3.7+** installed.

```bash
python file_organizer.py
```

---

## ⚙️ Usage

### 🧩 Basic Usage
Organize all files in the current directory:
```bash
python file_organizer.py
```

Organize a specific folder:
```bash
python file_organizer.py "C:\Users\Rama\Downloads"
```

---

### 🧪 Dry Run (Preview Only)
Preview the changes without actually moving files:
```bash
python file_organizer.py --dry-run
```

---

### ⚙️ Configuration Mode
Add or remove custom categories interactively:
```bash
python file_organizer.py --config
```
Example:
```
1. List current categories
2. Add new category
3. Remove category
4. Save configuration
5. Exit configuration
```

---

### ⏪ Undo Last Operation
Revert the last organization (restores files to original location):
```bash
python file_organizer.py --undo
```

---

### 🧹 Clean Empty Folders
Remove any empty directories created during organization:
```bash
python file_organizer.py --clean
```

---

## 📝 Log File
All actions are recorded in a log file:
```
organizer_log.txt
```

Example:
```
--- File Organization Log ---
Timestamp: 2025-11-05 13:45:22
Directory: C:\Users\Rama\Downloads
Files moved: 8
Moved files:
  photo.jpg -> Images/photo.jpg
  resume.pdf -> Documents/resume.pdf
----------------------------------------
```

---

## 🧠 Configuration File

Your custom file type settings are stored in:
```
organizer_config.json
```

Example:
```json
{
  "Images": [".jpg", ".png", ".jpeg"],
  "Documents": [".pdf", ".txt", ".docx"],
  "Videos": [".mp4", ".avi"]
}
```

You can manually edit this file anytime.

---

## 💡 Example Commands

| Command | Description |
|----------|-------------|
| `python file_organizer.py` | Organize current directory |
| `python file_organizer.py "C:\Users\Rama\Desktop"` | Organize specific folder |
| `python file_organizer.py --dry-run` | Preview actions only |
| `python file_organizer.py --undo` | Undo last organization |
| `python file_organizer.py --clean` | Remove empty directories |
| `python file_organizer.py --config` | Manage custom categories |

---

## 🧑‍💻 Author

**Rama**  
🎓 Engineering Student & Freelancer  
💼 Passionate about automation, scripting, and creative workflows.  
📧 [Your Email or Portfolio Link]

---

## 📜 License

This project is open source under the **MIT License**.  
Feel free to use, modify, and distribute it.
