# SimpleAnalogClockFont
A simple true type font including a glyph for all 720 minutes of an analog clock.
## Preview
![Gif](clock_showcase.gif)
## Indexing
The glyphs are located in the Private Use Area, starting at U+E000.
```
U+E000 → 00:00
U+E001 → 00:01  
U+E002 → 00:02  
…  
U+E03B → 00:59  
U+E03C → 01:00  
…  
U+E35F → 11:59
```

Formula:
```
index = hour * 60 + minute  
codepoint = 0xE000 + index
```

## Install Instructions:
### Linux
```
mkdir -p ~/.local/share/fonts
cp SimpleAnalogClockFont.ttf ~/.local/share/fonts/
fc-cache -f -v
```
### macOS
1. Download SimpleAnalogClockFont.ttf
2. Open with Font Book
3. Click **"Install Font"**
### Windows
1. Download SimpleAnalogClockFont.ttf
2. Right-click > Install
or
Open > "Install"
---
Licensed under CC-BY 4.0
