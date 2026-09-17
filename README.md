# Batch PDF Merger

Batch PDF Merger is a lightweight, purely client-side web application designed to append a single "master" PDF document to multiple target PDF files simultaneously. It processes everything directly in your web browser, ensuring your sensitive documents never leave your computer.

## 🚀 Features

* **100% Client-Side Processing:** Your files are processed locally in your browser. No data is uploaded to any server, guaranteeing absolute privacy and security.
* **Batch Processing:** Merge your master PDF with dozens of target files in one go.
* **Smart File Naming:** Output files are automatically renamed to include the `_merged.pdf` suffix (e.g., `document_merged.pdf`) so you can easily distinguish them from your originals without breaking file extensions.
* **Zip Archiving:** All processed PDFs are neatly bundled into a single `.zip` file for quick, one-click downloading.
* **File Optimization:** Optional structural optimization reduces file size by compressing internal PDF objects, ensuring files remain lightweight and perfectly legible on high-resolution (1080p/4K) screens.
* **Modern UI:** Clean, responsive interface built with Tailwind CSS.

## 🛠️ Technologies Used

* **HTML5 / JavaScript / CSS** - Core web technologies.
* **[Tailwind CSS](https://tailwindcss.com/)** - For modern, responsive styling.
* **[pdf-lib](https://pdf-lib.js.org/)** - For reading, modifying, and saving PDF documents directly in JavaScript.
* **[JSZip](https://stuk.github.io/jszip/)** - For creating the final ZIP archive containing all merged PDFs.

## 📖 How to Use

1. **Launch the App:** Simply double-click the `index.html` file to open it in any modern web browser (Chrome, Firefox, Edge, Safari). No installation or local server is required.
2. **Select Master PDF (Step 1):** Click the upload area or drag-and-drop the single PDF file that you want to append to the end of your other files.
3. **Select Target PDFs (Step 2):** Click the upload area or drag-and-drop multiple PDF files. These are the files that will receive the master PDF pages at their end.
4. **Settings (Step 3):** Check the "Optimize for 1080p Screens" box if you want the app to compress the internal PDF structure to save space.
5. **Process:** Click the **"Process & Download ZIP"** button.
6. **Download:** Wait for the progress bar to complete. A file named `Merged_PDFs.zip` will automatically download to your computer.

## ⚠️ Requirements

* A modern web browser with JavaScript enabled.
* An active internet connection is only required the very first time you load the page to fetch the external libraries (Tailwind, pdf-lib, JSZip) via CDN. The actual file processing happens offline.

## 🔒 Privacy Statement

Because this application relies entirely on browser-side JavaScript, **no files are ever uploaded, stored, or analyzed on any external server**. All document merging and zip creation happens using your device's local memory and processing power.
