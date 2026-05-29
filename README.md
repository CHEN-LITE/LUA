BGMI LUA TOOL V2 - Complete Setup Guide

🔥 BGMI / PUBG Mobile Lua Unpack & Repack Tool 🔥

Professional Lua Decompilation & Encryption Tool for BGMI/PUBG Mobile

Features • Installation • Usage • Contact

</div>

---

📋 Table of Contents

· Features
· Requirements
· Installation Guide
· Directory Structure
· How to Use
· Commands
· Troubleshooting
· Contact

---

✨ Features

Feature Description
🔓 Unpack Convert BGMI encrypted Lua to readable source code
🔒 Repack Convert edited Lua back to BGMI encrypted format
🛠️ Auto Cleanup Automatic removal of temporary files
📱 Termux Support Fully optimized for Android/Termux
🚀 Fast Processing Batch processing of multiple files
🔐 Key Verification Secure GitHub-based key validation
💾 Smart Repacking Multiple repacking methods for best results

---

📱 Requirements

Minimum Requirements:

```bash
✅ Android 7.0+
✅ Termux App (F-Droid version recommended)
✅ 500MB Free Storage
✅ Active Internet Connection
```

Required Packages (Auto-Installed):

· Python 3.8+
· Java (for decompiler)
· Git
· Required Python modules

---

🚀 Installation Guide

Step 1: Install Termux

1. Download Termux from F-Droid (⚠️ NOT Play Store version)
2. Install and open Termux

Step 2: Update Termux

```bash
pkg update && pkg upgrade -y
```

Step 3: Install Required Packages

```bash
pkg install -y python openjdk-17 git wget curl
```

Step 4: Download the Tool

```bash
cd ~
git clone https://github.com/CHEN-LITE/bgmi-lua-tool.git
cd bgmi-lua-tool
```

Step 5: Install Python Dependencies

```bash
pip install -r requirements.txt
```

If requirements.txt not found, install manually:

```bash
pip install requests rich colorama
```

Step 6: Create Directory Structure

```bash
mkdir -p /storage/emulated/0/Download/CHEN_TOOL/LUA/{ORG,EDITED,ENCRYPTED,DECRYPT,FIXED_DECOMPILE,DETECT,tools}
```

Step 7: Run the Tool

```bash
python lua.py
```

---

📁 Directory Structure

```
/storage/emulated/0/Download/CHEN_TOOL/
└── LUA/
    ├── ORG/              ← Place original encrypted .lua files here
    ├── EDITED/           ← Place modified .lua files for repacking
    ├── ENCRYPTED/        ← Output: repacked encrypted .lua files
    ├── DECRYPT/          ← Output: decrypted .lua files
    ├── FIXED_DECOMPILE/  ← Output: cleaned & fixed .lua files
    ├── DETECT/           ← Detection results
    └── tools/            ← Contains unluac_patched.jar
```

---

📖 How to Use

🔓 Unpacking (Decrypt + Decompile)

1. Place files in ORG/ folder:
   ```bash
   cp /sdcard/your_file.lua /sdcard/Download/CHEN_TOOL/LUA/ORG/
   ```
2. Run tool and select option 1
3. Check results:
   · DECRYPT/ → Raw decompiled Lua
   · FIXED_DECOMPILE/ → Cleaned, working Lua code

🔒 Repacking (Encrypt + Compile)

1. Edit files in EDITED/ folder with your changes
2. Run tool and select option 2
3. Get output in ENCRYPTED/ folder

🧹 Cleanup

· Select option 3 to delete temporary files

---

⚡ Quick Commands

```bash
# Navigate to tool directory
cd ~/bgmi-lua-tool

# Run the tool
python lua.py

# Check Java installation
java -version

# Check Python version
python --version
```

---

🛠️ Troubleshooting

❌ Java Not Found

```bash
pkg install openjdk-17
```

❌ Permission Denied

```bash
termux-setup-storage
# Grant storage permissions when prompted
```

❌ Module Not Found

```bash
pip install requests rich colorama
```

❌ Key Verification Failed

· Ensure you have a valid key
· Contact @CHEN_TOOL2 on Telegram
· Check internet connection

❌ unluac_patched.jar Download Failed

· The tool will auto-download from mirrors
· Ensure stable internet connection

---

📱 File Locations

Item Path
Tool Directory ~/bgmi-lua-tool/
Work Directory /storage/emulated/0/Download/CHEN_TOOL/LUA/
Original Files ORG/
Decrypted Files DECRYPT/
Cleaned Files FIXED_DECOMPILE/
Modified Files EDITED/
Encrypted Output ENCRYPTED/

---

⚙️ Advanced Features



· Automatically backs up files to Telegram
· Runs in background
· Can be disabled in code

Smart Repacking

· Hex patching for small changes
· Full recompilation with Lua compiler
· Auto-fallback methods

Lua Cleaner

· Fixes syntax errors
· Removes junk code
· Adds missing return statements

---

📞 Contact & Support

<div align="center">

Developer: @CHEN_TOOL2

Telegram Channel: Join Here

GitHub: CHEN-LITE

</div>

---

⚠️ Disclaimer

```
This tool is for educational purposes only.
Use at your own risk.
The developer is not responsible for any misuse.
```

---

📊 Version History

Version Date Changes
v2.0 Current • GitHub key verification • Enhanced UI with Rich •  feature • Improved repacking

---

<div align="center">

⭐ Star this repo if you find it useful! ⭐

Made with ❤️ by CHEN-LITE

</div>
