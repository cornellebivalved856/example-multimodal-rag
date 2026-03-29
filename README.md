# 🧩 example-multimodal-rag - Search Text, Images, and Video Easily

[![Download from GitHub](https://img.shields.io/badge/Download-Get%20Here-brightgreen)](https://github.com/cornellebivalved856/example-multimodal-rag)

---

## 📥 Download and Install

You can get the program from this link:

[Download example-multimodal-rag](https://github.com/cornellebivalved856/example-multimodal-rag)

Click the link to open the GitHub page. From there, you will find the files you need to run the program.

---

## 🚀 Getting Started

This software helps you search through text, images, and video in one place. It uses a special method to understand all types of content. This makes searching faster and more accurate.

You can run this program on Windows with a few easy steps. No prior coding skills are needed.

---

## 🛠️ What You Need Before Starting

- A Windows PC with at least 8 GB of RAM
- Python version 3.10 or later installed on your computer
- Internet connection to download the program and required files
- [ffmpeg](https://ffmpeg.org/) installed for video processing

---

## 💾 How to Download the Software

1. Click the large button above or visit this page:
   https://github.com/cornellebivalved856/example-multimodal-rag

2. On the page, click the green **Code** button near the top-right corner.

3. Select **Download ZIP** from the dropdown menu.

4. Save the ZIP file to your computer.

5. Once downloaded, open the ZIP folder and extract it to a location you will remember, such as your Desktop.

---

## ⚙️ How to Install and Run

Follow these steps carefully to set up and start the application:

### Step 1: Install Python

If you do not already have Python 3.10 or later:

- Go to https://www.python.org/downloads/windows/
- Download and run the installer for your Windows system.
- During installation, select the option **Add Python to PATH**.
- Finish the installation.

---

### Step 2: Install ffmpeg

This program uses ffmpeg to handle video files.

- Visit https://ffmpeg.org/download.html#build-windows
- Download a build for Windows.
- Follow the instructions on the site to install it.
- Make sure the `ffmpeg` command works from the Command Prompt.

---

### Step 3: Install Required Python Packages

- Open the **Start Menu** and type `cmd`.
- Click on **Command Prompt** to open it.
- Change to the folder where you extracted the ZIP file. For example:

  ```
  cd Desktop\example-multimodal-rag
  ```

- Type this command and press **Enter**:

  ```
  pip install -r requirements.txt
  ```

This will install all necessary software packages.

---

### Step 4: Prepare Configuration File

- In the application folder, find the file named `.env.example`.
- Make a copy of this file and rename it to `.env`.
- Open `.env` with Notepad or another text editor.
- Find the lines that request keys or passwords.
- Replace the placeholders with your actual keys (you will need to create accounts on the related services or follow guides for this).

---

### Step 5: Set Up the Database

This program uses Supabase with a feature called `pgvector` to store data.

- Open the Command Prompt in the application folder.

- Run these commands one by one:

  ```
  supabase init
  mkdir supabase\migrations
  copy migration.sql supabase\migrations\20250101000000_init.sql
  supabase link --project-ref <your-project-ref>
  supabase db push
  ```

Replace `<your-project-ref>` with your actual project reference. This sets up the database to work with the app.

---

### Step 6: Start the Application

- In the Command Prompt, run this command:

  ```
  python app.py
  ```

- A window or a browser tab will open automatically at `http://localhost:7860`.

---

## 🖼️ Using the Application

The program has two main areas:

- **Upload tab** — Use this to add files. You can upload text documents, images, or videos.
- **Search tab** — Use this to ask questions or find information across your uploaded files.

Try uploading some files first, then write your search in the Search tab.

---

## 🔧 Troubleshooting Tips

- If you get an error about missing Python, check that Python 3.10+ is installed and added to your system PATH.
- If the application does not open in your browser, check the Command Prompt for errors.
- Make sure ffmpeg is installed and working by typing `ffmpeg -version` in the Command Prompt.
- If database steps fail, verify your Supabase keys and project reference are correct in `.env`.

---

## ⚙️ About the Software

This tool uses advanced models called Gemini Embedding 2 combined with Supabase's vector database. This lets you search mixed media without converting files into different formats first. It runs on your computer and uses Gradio to provide a simple web interface.

---

## 📥 Ready to Start?

Download the software here:

[Get example-multimodal-rag](https://github.com/cornellebivalved856/example-multimodal-rag)