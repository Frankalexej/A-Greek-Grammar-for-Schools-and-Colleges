# HA-A-Greek-Grammar-for-Schools-and-Colleges
**J. Hadley & F. D. Allen (1884)**  *A Greek Grammar for Schools and Colleges*

This is an **auxiliary HTML-based reader** for navigating the Greek grammar book by Hadley and Allen. It provides a convenient interface for:

- 🔍 **Searching entries** by number (e.g., grammar section `35`),
- 📖 **Turning pages**,
- 🔢 **Jumping directly to any page** (including front matter or appendices),
- 🖼️ **Viewing scanned page images**.

---

## 📁 Features

- **Entry Search**: Enter a grammar entry number to jump to the page pair containing it.
- **Page Navigation**:
  - "⟵" / "⟶" buttons to flip through pages.
  - Page input for jumping directly to any page.
- **Fallback Handling**: If scanned images are missing, the app displays the page range text.

---

## 🔧 How It Works

- Grammar book pages are stored as `pages/X.png` (e.g., `2.png`).
- Each even-numbered page starts a grammar entry range, and the following odd page ends it (e.g., `[26` to `33]`).
- An OCR-generated and manually checked list (`entryRanges`) maps entries to page ranges.
- JavaScript handles all navigation logic; no server required.

---

## 🗂️ Files

- `grammar_checker.html`: Main interface
- `grammar_checker.js`: Core JavaScript logic for search and navigation
- `grammar_checker.css`: Responsive styling
- `pages/`: Folder containing page images (`8.png`, `9.png`, …)
- `preprocess`: Folder that contain codes to reformat from jp2 as downloadable from Internet Archive to png
---

## 📦 How to Use

1. Download resource from Internet Archive (https://archive.org/download/cu31924099427886/cu31924099427886_jp2.zip). 
2. Decompress it to the project directory. 
3. Run `preprocess/jp2_to_png.py` to reformat the resource. After running `/pages` directory are created and reformatted files are there.
4. I'm happy to transmit the reformatted files if you have any problem with it. I did not put it here because of its size. They are open source anyway. 
5. Open `grammar_checker.html` in any modern web browser.
6. Start searching entries or flipping through the grammar!

---

## 📘 Source Material

**J. Hadley and F. D. Allen**  
*A Greek Grammar for Schools and Colleges*  
Boston: Ginn & Heath, 1884

Scanned and digitized by Cornell University Library. 

---

## 📝 License

This project is distributed for non-commercial, academic use only. Original text is public domain.
