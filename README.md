# DiscordStatus

![Python](https://img.shields.io/badge/Python-3-3776AB?logo=python&logoColor=white)
![Tkinter](https://img.shields.io/badge/GUI-Tkinter-informational)
![Platform](https://img.shields.io/badge/platform-Windows-0078D6?logo=windows&logoColor=white)

A tiny Windows desktop app that lets you set a **custom text as its window title**, so you can show whatever you want as your "Playing…" activity on Discord.

![DiscordStatus window](https://github.com/ludenelenterrador/DiscordStatus/assets/134003146/c1890323-c33f-4638-985d-9fb90f216d28)

![Custom status on Discord](https://github.com/ludenelenterrador/DiscordStatus/assets/134003146/76c43aa4-07ec-4990-a760-5a172718ce75)

## Features

- Type any text and press **Actualizar Título** to update the window title instantly
- Lightweight single-file app (~50 lines of Python)
- Ready-made Windows executable in [`dist/`](dist/)

## Download

- **Installer (Win64/32):** [SetupDiscordStatus.exe](https://luden.x10.mx/SetupDiscordStatus.exe)
- **Portable:** [`dist/main.exe`](dist/main.exe)

## Run from source

```bash
pip install pillow requests
python main.py
```

Build the executable yourself with [PyInstaller](https://pyinstaller.org/):

```bash
pip install pyinstaller
pyinstaller main.spec
```

## How it works

The app is a small Tkinter window with a text field. When you click the button, it calls `window.title(text)`. Add the program to Discord under **Settings → Activity Privacy → Registered Games** and Discord will display it as your current activity.

## Tech stack

Python · Tkinter · Pillow · Requests · PyInstaller

---

Made by [Luden](https://github.com/ludenelenterrador)
