# ⚡ Speed Test App!

<p align="center"><img src="https://github.com/user-attachments/assets/52c44ac1-81b1-4ad5-8afe-08e0a5305f04" alt="speedmeter app" width="200"></p>



A simple and lightweight app to measure your internet **download** and **upload** speeds using Python and the `speedtest` module. Optionally, you can convert it into a standalone `.exe` with a custom icon.

---

## 🚀 Features

- Check download and upload speeds
- Lightweight and fast
- No need for a browser
- Optionally packaged as a Windows executable
- Add your own icon to the `.exe` file

---

## 📦 Requirements

- Python 3.11+
- pip

Install dependencies:

```bash
pip install pyinstaller
```

---

## 🖥️ Usage

To run from the command line:

```bash
python speed.py
```

Sample output:

```
Download speed: 55.32 Mbps
Upload speed: 48.45 Mbps
```

---

## 🛠️ Build as Executable (.exe)

You can package it into a standalone Windows executable with a custom icon.

### 1. Convert Icon (if needed)
Ensure your icon is in `.ico` format. You can convert `.png` to `.ico` using [https://convertio.co/png-ico/](https://convertio.co/png-ico/).

Place `speed.ico` in the same directory as your Python script.

### 2. Create Executable

Run this in the terminal:

```bash
pyinstaller --onefile --icon=speedicon.ico speed.py
```

### 3. Locate the Executable

After building, the `.exe` file will be found in the `dist/` folder:

```
dist/speed.exe
```

Double-click to run, or use from the terminal.

---

## 🧹 Optional Clean Build

To remove previous builds:

```bash
rm -r build dist speed.spec
```

Then re-run PyInstaller.

---

## 📄 License

This project is open-source under the [MIT License](LICENSE).

---

## 🙌 Acknowledgements
- [PyInstaller](https://pyinstaller.org/) for packaging
