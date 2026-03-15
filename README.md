# FlameVortex Ultimate Decoder

<div align="center">

**A powerful Python obfuscation decoder toolkit with 9 professional decoders**

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Version](https://img.shields.io/badge/Version-1.0-orange.svg)](https://github.com/FlameVortex)

[Features](#features) • [Installation](#installation) • [Usage](#usage) • [Decoders](#decoders) • [Documentation](#documentation)

</div>

---

## 🎯 Overview

FlameVortex Encryption Decoder is a comprehensive toolkit for analyzing and decoding obfuscated Python code. Whether you're dealing with Cython extensions, Marshal layers, or complex multi-stage encodings, this tool provides the solution.


### 🛑 All Decoder

- **Cython .so File Decoder** 
- **Marshal Decoder** 
- **Lambda Marshal+Zlib+Base64 Decoder** 
- **Base64 Decoder** 
- **Zlib Decoder** 
- **Hexadecimal Decoder** 
- **Base64 + Zlib Decoder** 
- **Base64 + Marshal Decoder** 
- **Exec Marshal+Zlib+Base64 Decoder** 

---




### Key Highlights

- **9 Specialized Decoders** covering all major obfuscation techniques
- **Automatic Multi-Layer Processing** with detailed analysis
- **Professional Output** with formatted headers and metadata
- **Secure Access Control** via Firebase authentication
- **Cross-Platform** support (Termux, Linux, Kali)
- **Cython Compiled** for speed and security

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 🔧 Core Features
- 9 professional decoders
- Multi-layer support
- Dual output modes
- Color-coded interface
- Progress tracking
- Error recovery

</td>
<td width="50%">

### 🔐 Security
- Unique device keys
- Access control system
- Secure key storage
- Real-time validation
- Cython protected code

</td>
</tr>
</table>

### 📊 Output Capabilities

- **Terminal Mode**: Quick preview with colored output
- **File Mode**: Professional headers with complete metadata
- **Analysis**: Entropy calculations, hash verification, layer counting
- **Disassembly**: Automatic Python bytecode disassembly

---

## 🛠 Decoders

<details>
<summary><b>1. Cython .SO File Decoder</b></summary>

Extracts and decodes encrypted code from Cython-compiled shared object files.

**Features:**
- Base64 pattern extraction
- Multiple candidate testing
- Automatic Zlib handling
- Marshal disassembly

**Use Case:** Reverse engineering Cython extensions
</details>

<details>
<summary><b>2. Marshal Layer Decoder</b></summary>

Recursively unpacks multi-layer Marshal obfuscation.

**Features:**
- Automatic layer detection
- Nested payload identification
- Layer counting
- Full disassembly

**Use Case:** Nested `marshal.loads()` obfuscation
</details>

<details>
<summary><b>3. Lambda Marshal+Zlib+Base64 Decoder</b></summary>

Advanced decoder with comprehensive analysis capabilities.

**Features:**
- Reverse byte processing
- Entropy analysis
- Hash verification
- String extraction
- Suspicious function detection

**Use Case:** Complex Lambda-style obfuscation
</details>

<details>
<summary><b>4. Base64 Decoder</b></summary>

Simple, reliable Base64 decoding.

**Use Case:** Standard Base64 encoded files
</details>

<details>
<summary><b>5. Zlib Decoder</b></summary>

Zlib decompression with UTF-8 conversion.

**Use Case:** Compressed Python code
</details>

<details>
<summary><b>6. Hexadecimal Decoder</b></summary>

Hex to text conversion with formatting support.

**Use Case:** Hexadecimal obfuscated code
</details>

<details>
<summary><b>7. Base64 + Zlib Decoder</b></summary>

Two-stage decoder: Base64 → Zlib

**Use Case:** Combined Base64 and Zlib encoding
</details>

<details>
<summary><b>8. Base64 + Marshal Decoder</b></summary>

Base64 → Marshal → Disassembly pipeline

**Use Case:** Base64-wrapped Marshal objects
</details>

<details>
<summary><b>9. Normal Marshal+Zlib+Base64 Decoder</b></summary>

Detects and decodes `b64decode()` patterns.

**Use Case:** Standard Python obfuscation chains
</details>

---

## 📥 Installation

### Quick Install (Termux/Linux)

```bash
# Clone repository
git clone https://github.com/FlameVortex/Flame-Decoder.git
cd Flame-Decoder

# Install dependencies
pip install -r requirements.txt

# Run the tool
python decoder.py
```


### Requirements

| Package | Version | Purpose |
|---------|---------|---------|
| Python | 3.7+ | Runtime |
| colorama | 0.4.6+ | Terminal colors |
| requests | 2.28.0+ | API calls |

### Platform Compatibility

✅ **Supported:**
- Termux (Android - ARM/ARM64)
- Linux x86_64
- Kali Linux
- Ubuntu/Debian

<details>
<summary><b>Detailed Installation Guide</b></summary>

### For Termux (Android)

```bash
# Update packages
pkg update && pkg upgrade -y

# Install Python and Git
pkg install python git -y

# Clone repository
cd ~
git clone https://github.com/FlameVortex/Flame-Decoder.git
cd Flame-Decoder

# Install runtime dependencies
pip install -r requirements.txt

# Run the tool
python decoder.py
```

### For Linux/Kali

```bash
# Update system
sudo apt update && sudo apt upgrade -y

# Install Python and Git
sudo apt install python3 python3-pip git -y

# Clone repository
git clone https://github.com/FlameVortex/Flame-Decoder.git
cd Flame-Decoder

# Install dependencies
pip3 install -r requirements.txt

# Run the tool
python3 decoder.py
```

### Troubleshooting Installation

**Issue: "cannot open shared object file"**
```bash
# Install Python development files
# For Termux:
pkg install python-dev

# For Linux:
sudo apt install python3-dev
```

**Issue: "No module named 'colorama'"**
```bash
pip install -r requirements.txt --force-reinstall
```

</details>

---

## 🚀 Usage

### Quick Start

```bash
# Run the compiled tool
python decoder.py

# Or if you have multiple Python versions
python3 decoder.py
```

### Workflow

```
1. Approval Check
   ↓
2. Select Decoder (1-9)
   ↓
3. Enter File Path
   ↓
4. Choose Output Mode
   ↓
5. View Results
```

### Example Session

```bash
$ python ultimate_decoder*.so

==========================================
    🔓 ACCESS GRANTED — KEY APPROVED
==========================================

╔═════════════════════════════════════════════════════════════╗
║     SELECT DECODER TYPE                                     ║
╠═════════════════════════════════════════════════════════════╣
║  1 → Cython .SO File Decoder                                ║
║  2 → Marshal Layer Decoder                                  ║
║  3 → Lambda Marshal+Zlib+Base64 Decoder                     ║
║  4 → Base64 Decoder                                         ║
║  5 → Zlib Decoder                                           ║
║  6 → Hexadecimal Decoder                                    ║
║  7 → Base64 + Zlib Decoder                                  ║
║  8 → Base64 + Marshal Decoder                               ║
║  9 → Normal Marshal+Zlib+Base64 Decoder                     ║
╚═════════════════════════════════════════════════════════════╝

► Select decoder type: 4
► Enter file path: encoded.py

╔═══════════════════════════════════════╗
║     SELECT OUTPUT MODE                ║
╠═══════════════════════════════════════╣
║  1 → Print decoded result             ║
║  2 → Save decoded result to TXT       ║
╚═══════════════════════════════════════╝

► Select option: 1

[✓] Base64 decode successful

╔═══════════════════════════════════════╗
║     ✓ DECODE SUCCESSFUL ✓             ║
╚═══════════════════════════════════════╝
```

---


### Getting Approved

If you see:

```
==========================================
    🔒 ACCESS DENIED — KEY NOT APPROVED
==========================================

🔑 Your Key: ABC123DEF456...
👉 Message Admin to Approve Your Key.
```

**Steps:**
1. Copy your device key
2. Press ENTER (opens Telegram)
3. Send key to [@FlameVortex_TRS](https://t.me/FlameVortex_TRS)
4. Wait for approval (usually within 24 hours)
5. Re-run tool

---

## 📤 Output Formats

### Terminal Output
```
[⚙] Reading file...
[⚙] Attempting Base64 decode...
[✓] Base64 decode successful

═══════════════════════════════════════
DECODED RESULT
═══════════════════════════════════════

[decoded content here]

╔═══════════════════════════════════════╗
║     ✓ DECODE SUCCESSFUL ✓             ║
╚═══════════════════════════════════════╝
```

### File Output (with Header)
```
╔═══════════════════════════════════════════════════════════════╗
║                     DECODED FILE INFORMATION                  ║
╠═══════════════════════════════════════════════════════════════╣
║  Decoded by    : FlameVortex                                  ║
║  GitHub        : github.com/FlameVortex                       ║
║  Decoder Type  : Base64 Decoder                               ║
║  Decoded Time  : 2026-03-15 18:30:45                          ║
║  Source File   : example.py                                   ║
╚═══════════════════════════════════════════════════════════════╝

═══════════════════════════════════════════════════════════════
DECODED CONTENT
═══════════════════════════════════════════════════════════════

[Your decoded content here]
```

---

## 💡 Examples

### Example 1: Base64 File

**Input:** `encoded.py`
```
SGVsbG8gV29ybGQh
```

**Command:**
```bash
python decoder.py
# Select: 4
# File: encoded.py
# Output: Terminal
```

**Result:**
```
Hello World!
```

---

### Example 2: Marshal Layers

**Input:** `obfuscated.py`
```python
import marshal
exec(marshal.loads(b'\xe3\x00\x00\x00...'))
```

**Command:**
```bash
python decoder.py
# Select: 2
# File: obfuscated.py
# Output: Save to file
```

**Result:** Full disassembly with layer information

---

## 🔧 Advanced Usage

### Command Line Tips

```bash
# Run with Python 3 explicitly
python3 decoder.py

# Create an alias for easy access
alias decoder='python3 ~/Flame-Decoder/decoder.py

# Then just run
decoder
```

### Decoder Selection Guide

| File Type | Recommended Decoder |
|-----------|---------------------|
| `.so` files | Decoder 1 (Cython) |
| Marshal layers | Decoder 2 (Marshal) |
| Base64 only | Decoder 4 (Base64) |
| Zlib only | Decoder 5 (Zlib) |
| Base64+Zlib | Decoder 7 |
| Base64+Marshal | Decoder 8 |
| b64decode() pattern | Decoder 9 |
| Unknown/Complex | Try Lambda (Decoder 3) |

---

## 🐛 Troubleshooting

<details>
<summary><b>Access Denied</b></summary>

**Problem:** Key not approved

**Solution:** Send key to admin via Telegram [@FlameVortex_TRS](https://t.me/FlameVortex_TRS)
</details>

<details>
<summary><b>Module Not Found</b></summary>

**Problem:** Missing dependencies

**Solution:**
```bash
pip install -r requirements.txt
```
</details>

<details>
<summary><b>Cannot Execute .so File</b></summary>

**Problem:** Wrong platform or missing Python dev files

**Solution:**
```bash
# For Termux
pkg install python-dev

# For Linux
sudo apt install python3-dev
```
</details>

<details>
<summary><b>ImportError: libpython not found</b></summary>

**Problem:** Python shared library missing

**Solution:**
```bash
# Reinstall Python with shared library support
# For Termux
pkg reinstall python

# For Linux
sudo apt install --reinstall python3
```
</details>

<details>
<summary><b>Payload Not Found</b></summary>

**Problem:** Wrong decoder or corrupted file

**Solution:**
- Try different decoders
- Verify file integrity
- Check file encoding
</details>

<details>
<summary><b>Connection Error</b></summary>

**Problem:** No internet connection

**Solution:**
- Check network connection
- Approval system requires internet
- Retry after connection restored
</details>

---

## 📖 Documentation

- **[Installation Guide](INSTALL.md)** - Detailed setup instructions
- **[License](LICENSE)** - MIT License details

---

## 🤝 Contributing

This project is distributed as compiled Cython code. For feature requests or bug reports:

- 🐛 [Report Issues](https://github.com/FlameVortex/Flame-Decoder/issues)
- 💬 [Contact on Telegram](https://t.me/FlameVortex_TRS)
- 📧 Email: flamevortex@example.com

---

## 💬 Support

| Channel | Link |
|---------|------|
| Telegram | [@FlameVortex_TRS](https://t.me/FlameVortex_TRS) |
| GitHub Issues | [Report Bug](https://github.com/FlameVortex/Flame-Decoder/issues) |
| Email | flamevortex@example.com |

---

## 📜 License

MIT License - See [LICENSE](LICENSE) file

```
Copyright (c) 2026 FlameVortex

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

---

## ⚠️ Disclaimer

**For educational and authorized security research only.**

✅ Security research • ✅ Malware analysis • ✅ Code auditing  
❌ Unauthorized access • ❌ IP theft • ❌ Illegal activities

**The developer is not responsible for misuse.**

---

## 👨‍💻 Credits

**Developer:** FlameVortex  
**GitHub:** [@FlameVortex](https://github.com/FlameVortex)  
**Telegram:** [@FlameVortex_TRS](https://t.me/FlameVortex_TRS)

### Technology Stack

- **Language:** Python 3.7+
- **Compilation:** Cython
- **UI:** Colorama

### Version History

- **v1.0** (2026-03-15) - Personal Edition
  - 9 professional decoders
  - Cython compilation
  - Approval system
  - Unified design

---

<div align="center">

**🔥 Made ❤️ by FlameVortex 🔥**

If you find this useful, please ⭐ star the repository!

</div>
