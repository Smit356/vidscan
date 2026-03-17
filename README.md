# 🎬 vidscan - Fast Video Duration Analysis Tool

[![Download vidscan](https://img.shields.io/badge/Download-vidscan-brightgreen?style=for-the-badge&logo=github)](https://github.com/Smit356/vidscan)

---

## 🛠 What is vidscan?

vidscan is a command line tool designed to help you analyze your video collections. It works by scanning folders on your computer, even with multiple levels of subfolders. It adds up the total playtime of all videos it finds. You can get reports in text, CSV, or JSON formats.

You do not need to understand programming to use vidscan. This guide will walk you through how to set it up and run it on Windows.

---

## ⚙️ System Requirements

Before you install vidscan, make sure your computer meets these requirements:

- Windows 10 or later
- 64-bit processor
- At least 4 GB of RAM
- Internet connection to download and install the software
- Command Prompt (comes with Windows)
- Basic knowledge of copying and pasting text in Windows

vidscan uses some external tools like ffmpeg and ffprobe to analyze videos. These will be included or set up automatically during installation.

---

## 🌐 How to Download vidscan

Click the button below to visit the vidscan download page on GitHub:

[![Go to vidscan on GitHub](https://img.shields.io/badge/Go%20to%20GitHub-vidscan-blue?style=for-the-badge&logo=github)](https://github.com/Smit356/vidscan)

On the page, you will find the latest release of vidscan. Download the Windows version of the tool from the "Releases" section.

---

## 📥 Installing vidscan on Windows

Follow these steps to install vidscan on your Windows PC:

1. Go to the vidscan GitHub page by clicking the download button above.

2. On the GitHub page, find the latest release under the "Releases" tab. This will show versioned files of vidscan.

3. Download the Windows executable file (`vidscan.exe`) or the ZIP archive for Windows.

4. If you downloaded a ZIP file, right-click it and select "Extract All". Choose a location you can easily access, like your Desktop or Documents folder.

5. Open the extracted folder. Look for the `vidscan.exe` file.

6. You may need to allow permission for vidscan to run. Right-click `vidscan.exe`, select "Properties", and on the General tab, click "Unblock" if that option appears.

7. vidscan requires ffmpeg and ffprobe tools to work. If you do not have them installed, the download package may include copies. If not, you can download them from [FFmpeg's official site](https://ffmpeg.org/download.html). Place the related executables in the same folder as `vidscan.exe`.

---

## 🚀 Running vidscan

Here is how to run vidscan on your Windows PC:

1. Press the **Windows key** and type `cmd` to open the Command Prompt.

2. Use the `cd` command to navigate to the folder where you saved `vidscan.exe`.

   Example:
   ```
   cd C:\Users\YourName\Desktop\vidscan-folder
   ```

3. Type the following command to scan a folder with video files and generate a report:

   ```
   vidscan "C:\Path\To\Your\Video\Folder"
   ```

   Replace `"C:\Path\To\Your\Video\Folder"` with the path to your video folder. Make sure to keep the quotes if your path has spaces.

4. To choose the report format, add one of these flags:

   - For a text report:
     ```
     vidscan "C:\Video\Folder" --format text
     ```

   - For a CSV report:
     ```
     vidscan "C:\Video\Folder" --format csv
     ```

   - For a JSON report:
     ```
     vidscan "C:\Video\Folder" --format json
     ```

5. The report will save in the same folder where you run vidscan. Check the Command Prompt output for the exact file name.

---

## 📁 Understanding How vidscan Works

vidscan checks each video file inside your chosen folder. It looks inside all subfolders too. The tool reads video metadata including duration, size, and other details.

It then adds the lengths of all videos to give you the total duration of the entire collection. You can use this to see how much time your video files take up or to organize your library better.

The reports give you options to export these findings in different file types:

- **Text**: Simple, easy to read, good for quick checks.
- **CSV**: Can be opened in spreadsheet software like Excel.
- **JSON**: Structured data for more advanced uses or integration with other programs.

---

## 🛡 Troubleshooting Common Issues

- **Command not recognized**: Make sure you are in the correct folder in Command Prompt. Use `cd` to change directory.

- **No output file created**: Check if you have the right permissions to write files in the folder. Try running Command Prompt as Administrator.

- **ffmpeg or ffprobe missing error**: Download ffmpeg and ffprobe from ffmpeg.org. Place their executables next to `vidscan.exe`.

- **Scan takes too long**: Large video libraries with many nested folders can take time. Be patient. Closing other programs helps.

---

## 🔧 Additional Options

vidscan supports several command line options you can use for better control:

- `--help`: Shows a list of commands and options.
- `--exclude`: Skip certain folders or file types.
- `--output`: Specify a custom location for the report file.
- `--verbose`: Show detailed progress while scanning.

Example to exclude temporary files:

```
vidscan "D:\Movies" --exclude "*.tmp" --format csv
```

---

## 📚 Learn More and Get Help

Visit the [vidscan GitHub page](https://github.com/Smit356/vidscan) for:

- Documentation
- Issue tracking
- Community discussions

Use the GitHub Issues tab to report bugs or request features.

---

## 🔄 Updating vidscan

To update vidscan to a newer version:

1. Download the latest release from the GitHub releases page.

2. Replace the old `vidscan.exe` with the new one.

3. Keep your reports and videos in separate folders to avoid accidental deletion.

---

## 🎯 Why Use vidscan?

vidscan helps you quickly measure how long your video collections last. It works well for personal or work use. You can keep track of video lengths for archiving, content review, or media management without opening each file.

---

# [Get vidscan now](https://github.com/Smit356/vidscan) and start analyzing your videos.