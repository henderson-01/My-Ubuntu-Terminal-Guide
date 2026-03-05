# 🐧 My Ubuntu Terminal Guide for Beginners

### 40 Essential Commands to Master the Command Line

This repository contains a curated list of my most used Ubuntu terminal commands. Whether you are managing a local machine or a remote server, these commands will be your bread and butter.

> [!IMPORTANT]
> **How to Read the Placeholders:**
> When you see **`<text in brackets>`**, this is a **placeholder**.
> * **Do not type the `< >` symbols.**
> * **Replace the text inside** with your actual file name, folder name, or address.
> * *Example:* To change to a folder named "Documents," you would type: `cd Documents` (not `cd <Documents>`).
> 
> 

---

## 📂 Navigation & File Basics

| Command | Description | Expected Output |
| --- | --- | --- |
| `pwd` | **P**rint **W**orking **D**irectory. Shows your current location. | A path like `/home/username/Documents`. |
| `ls` | **L**i**s**t. Shows files and folders in your current spot. | A list of names. (Folders are usually blue). |
| `cd <dir>` | **C**hange **D**irectory. Moves you into a specific folder. | Command prompt updates to the new path. |
| `cd ..` | Moves you "up" one level to the parent folder. | You move back one step in the directory tree. |
| `clear` | Wipes the terminal screen of all old text. | A fresh, empty terminal window. |
| `mkdir <name>` | **M**a**k**e **D**irectory. Creates a new folder. | No output; use `ls` to verify. |
| `touch <file>` | Creates a new, completely empty file. | An empty file appears in the directory. |

## 🛠️ Managing Files & Text

| Command | Description | Expected Output |
| --- | --- | --- |
| `cp <src> <dest>` | **C**o**p**y a file to a new location or name. | A duplicate file is created. |
| `cp -r <src> <dest>` | **C**o**p**y **R**ecursively. Use this to copy **folders**. | A duplicate folder and all its contents. |
| `mv <old> <new>` | **M**o**v**e or **Rename**. Moves a file or changes its name. | File moves or name changes instantly. |
| `rm <file>` | **R**e**m**ove. Deletes a file **permanently**. | The file is deleted (no Trash bin!). |
| `rm -r <dir>` | **R**ecursive remove. Deletes a folder and everything inside. | The folder and its contents are gone. |
| `cat <file>` | Reads a file and displays the text on screen. | The text content spills into the terminal. |
| `nano <file>` | Opens a beginner-friendly text editor. | Terminal turns into a text editing interface. |
| `head <file>` | Shows only the first 10 lines of a file. | The beginning of a document. |
| `tail <file>` | Shows only the last 10 lines of a file. | The end of a document (useful for logs). |

## ⚡ System & Admin (Root Tools)

| Command | Description | Expected Output |
| --- | --- | --- |
| `sudo` | **S**uper**U**ser **DO**. Runs commands with admin rights. | Prompt for your password (characters stay hidden). |
| `sudo apt update` | Refreshes the list of available software updates. | Lines of "Get" and "Hit" from web servers. |
| `sudo apt upgrade` | Installs all available software updates. | A `[Y/n]` prompt to confirm the download. |
| `sudo apt install <pkg>` | Downloads and installs a new program. | Progress bars as software is set up. |
| `df -h` | **D**isk **F**ree. Shows available hard drive space. | Table showing Size, Used, and Available space. |
| `free -h` | Shows current RAM (memory) usage. | Summary of total, used, and free memory. |
| `top` | Real-time view of running processes. | A live list of CPU/RAM usage (Press `q` to exit). |
| `uname -a` | Displays detailed info about the Linux kernel. | Text string with OS version and architecture. |

## 🔍 Searching & Networking

| Command | Description | Expected Output |
| --- | --- | --- |
| `grep <text> <file>` | Searches for a word or phrase inside a file. | Highlights the lines where the text was found. |
| `find . -name <file>` | Searches for a file by name in the current spot. | The relative path to the file if found. |
| `history` | Shows a list of all commands you’ve typed. | A numbered list of your past activity. |
| `ping <site>` | Tests connection to a website (e.g., google.com). | Repeating response times (Press **Ctrl+C** to stop). |
| `ip addr` | Shows network connection info and IPs. | Look for `inet` to find your local IP address. |
| `wget <url>` | Downloads a file directly from a web link. | A progress bar as the file saves locally. |
| `man <command>` | Opens the **man**ual (help guide) for any command. | A full manual; press `q` to exit. |

## 🚀 Advanced Search & Troubleshooting

| Command | Description | Expected Output |
| --- | --- | --- |
| `htop` | Colorful, interactive process manager. | Visual dashboard of CPU, RAM, and tasks. |
| `du -sh <dir>` | **D**isk **U**sage. Shows total size of a folder. | A summary like `4.2G  /home/user/Videos`. |
| `locate <file>` | Quickly finds a file path (requires `plocate`). | A list of every location for that filename. |
| `grep -r "<txt>" <dir>` | Finds a word inside *all* files within a folder. | List of files and lines where text was found. |
| `alias <n>='<cmd>'` | Creates a custom shortcut for a long command. | No output; typing `<n>` runs the full command. |
| `lsusb` | Lists all connected USB devices. | Names of webcams, keyboards, and drives. |
| `lspci` | Lists all internal hardware (GPU, Wi-Fi). | Technical specs of internal components. |
| `journalctl -xe` | Shows the most recent system error logs. | Scrolling text showing system background tasks. |
| `history \| grep <txt>` | Searches your history for a specific command. | A list of every time you used that word. |
| `exit` | Closes the current terminal session. | Terminal window closes or logs you out. |

---

### 💡 Pro Tips

* **Tab Completion:** Type the first few letters of a file/folder and press `Tab` to autocomplete. It saves time and prevents typos!
* **Command History:** Use the `Up` and `Down` arrow keys to cycle through previous commands.
* **Stop/Kill:** Press `Ctrl + C` to force-stop a command that is currently running (like `ping` or `top`).
* **The Pipe (`|`):** Used to send the output of one command into another (e.g., `history | grep sudo`).
* **Safety First:** Use `rm -i <file>` to make the terminal ask for confirmation before deleting.

---

## ⚠️ Disclaimer 

This project is provided "as-is" without any warranty of any kind. I am not responsible for any issues, data loss, or "explosions" (code-related or otherwise) that may occur from using this software. **Use it at your own risk.**
