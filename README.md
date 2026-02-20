> **⚠️ This repository has been archived and moved.**
> 
> This project is now part of the comprehensive [CodeClause-Internship-Projects](https://github.com/patelritiq/CodeClause-Internship-Projects) repository.
> 
> Please visit the new repository for the latest version and all CodeClause internship projects.



# Textor: A Basic Text Editor ✍️

**Textor** is a lightweight, efficient text editor developed in Python using the `Tkinter` framework. It goes beyond basic note-taking by incorporating real-time spell-checking and word-count features, making it a practical tool for quick editing tasks and learning purposes.

---

## 🚀 Key Features
* **Real-time Spell Checking:** Automatically highlights misspelled words in **red** as you type, referencing a local dictionary file.
* **Essential File Operations:** Easily create **New** files, **Open** existing ones, and **Save** your work via an intuitive menu bar.
* **Live Word Count:** Instantly check the length of your document through the status bar.
* **Dynamic UI:** Features a responsive design with a wrapping text area and a live status bar for user feedback.

---

## 🛠️ Technical Stack
* **Language:** Python 3.x
* **GUI Framework:** Tkinter
* **Core Logic:** Event-driven programming with regex-based text processing.
* **Data Handling:** Local dictionary validation using `words.txt`.

---

## 🎮 How to Use
1. **Writing:** Type freely in the main text area.
2. **Spell Check:** Any word not found in the dictionary will be highlighted in red automatically.
3. **Menu Controls:**
    * **New:** Clear the editor for a fresh start.
    * **Open:** Browse and load `.txt` files from your computer.
    * **Save:** Save your current progress to a file.
    * **Word Count:** Click to see the total words in the status bar.
    * **Exit:** Safely close the editor.

---

## 💻 Installation & Setup

### 1. Requirements
Ensure you have Python installed. You will also need a `words.txt` file in the same directory as the script.

### 2. Generate the Dictionary (Optional)
If you do not have `words.txt`, you can generate it using `nltk` in Python:
```python
import nltk
nltk.download('words')
from nltk.corpus import words

with open("words.txt", "w") as file:
    for word in words.words():
        file.write(word + "\n")
```

### 3. Run the Application
1. **Clone the repo:**
   ```bash
   git clone https://github.com/patelritiq/Textor.git

2. **Run the script:**
   ```bash
   python textor.py
