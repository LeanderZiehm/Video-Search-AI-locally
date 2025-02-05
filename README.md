## 📂 Video Management Tool  

This project is a video management tool 🛠️ designed to help organize and search through large collections of videos stored in deeply nested directories.  

### ✨ Key Features:  
- 🗂 **File Parsing:** Automatically parses all file paths in the directory.  
- 🖼️ **Keyframe Extraction:** Extracts keyframes from each video for quick preview.  
- 🔑 **Keyword Generation:** Analyzes videos to generate meaningful keywords for better searchability.  
- 🔍 **Efficient Search:** Allows users to search by topic and retrieve the original file path.  

Developed as part of a marketing internship 🎓 to help the marketing department streamline video organization and improve productivity.

## Running the Project Locally

### Prerequisites:
1. **Clone the repository**  
   ```bash
   git clone https://github.com/LeanderZiehm/Video-Search-AI
   cd Video-Search-AI
   ```
   
2. **Install [Ollama](https://ollama.com/)**  
   Download and install Ollama from the official website.

3. **Run the LLaVA model**  
   ```bash
   ollama run llava
   ```

4. **Prepare video folder**  
   - Place your videos inside the `video/` folder.

5. **Install Python (if not installed)**  
   Download and install Python 3 from [here](https://www.python.org/downloads/).

6. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

### Running the Application:
1. **Process the videos**  
   ```bash
   python processVideos.py
   ```

2. **Start the main application**  
   ```bash
   python main.py
   ```

3. **Access the web interface**  
   Open your browser and go to:  
   ```
   http://127.0.0.1:5000/
   ```

Now you can use the application locally! 🚀

### Keyboard Shortcuts for the Application (Windows & Mac)

| **Shortcut (Windows)**   | **Shortcut (Mac)**         | **Function**                                                                 |
|---------------------------|----------------------------|-------------------------------------------------------------------------------|
| Ctrl + Click on video background | ⌘ + Click on video background | Selects a video (or deselects it).                                           |
| Ctrl + A                 | ⌘ + A                      | Selects or deselects all checkboxes.                                         |
| Ctrl + E                 | ⌘ + E                      | Opens the window for editing the keywords of selected videos.                |
| Escape                   | Escape                     | - Closes the editing window (if open) and saves changes.                     |
|                           |                            | - Deselects all checkboxes.                                                  |
| Ctrl + Up Arrow          | ⌘ + Up Arrow               | Scrolls immediately to the top of the page.                                  |
| Ctrl + Down Arrow        | ⌘ + Down Arrow             | Scrolls immediately to the bottom of the page.                               |

---

### 🔎 Search Bar  
Enter a keyword and press **Enter** to search for it.

#### Negative Search  
If you begin a keyword with `!`, the results will show all videos that do **not** contain that keyword.  
For example, with strict search and multiple keywords, you can use a negative search to find videos missing a specific keyword, like `!deggster`.

---

### ⚙️ Settings  
- **Strict Search:** Enable for exact matches.  
- **Search Path:** Also searches within file paths.  

---

### 🏷️ Manage Keywords  

#### Display  
Keywords are shown in the "Keywords" column.

#### Editing  
1. Select videos by clicking on them (the row will be highlighted).  
2. Click **Edit Selected** to open the keyword modal.  
3. Add new keywords or delete existing ones.  
4. Save changes by closing the modal.

---

### 📋 Video Table  
The table displays details about videos:

- **Preview:** Hovering over a thumbnail shows 5 frames of the video.  
- **Keywords:** Click on keywords to add/remove them from the search.  

#### Sorting 🔽🔼  
Click on a column header to sort by that column (ascending/descending).  
- **Date:** Creation date.  
- **Length:** Video duration in seconds.  
- **Size:** File size in MB.  
- **Aspect Ratio, FPS:** Technical details.