# 🔊 Simple Sound Player

This is a lightweight Python script to play `.mp3` sound files using `ffplay` (from the FFmpeg suite). It's useful for quick access to short audio clips via the terminal.

## 📦 Requirements

* Python 3.x
* FFmpeg (`ffplay` must be installed and available in your PATH)

You can install FFmpeg using your package manager:

```bash
# Debian/Ubuntu
sudo apt install ffmpeg

# Arch Linux
sudo pacman -S ffmpeg

# macOS with Homebrew
brew install ffmpeg
```

## 📁 Directory Structure

All sound files must be placed in:

```
/home/seva/projects/python/sounds/sounds
```

Each sound must be in `.mp3` format.

## ✨ Usage

```bash
python main.py <sound_name>
```

### Options

* `-h` — Show help message
* `-l` — List available sounds in the sounds directory

### Examples

Play a sound named `ping.mp3`:

```bash
python main.py ping
```

List available sounds:

```bash
python main.py -l
```

Show help:

```bash
python main.py -h
```

## ⚠️ Troubleshooting

If you get this error:

```
Command ffplay is not available, did you install ffmpeg?
```

Please make sure `ffplay` is installed and accessible in your system's PATH.

## 🛠 Customization

You can modify the `sounds_dir` variable at the top of the script to change the folder path where your `.mp3` files are stored.
