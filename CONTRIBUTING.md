# CONTRIBUTING
This isn't really in a good place for contributions right now.
But for my own notes:

- You probably don't want to do font dev under macOS. It aggressively caches fonts, which leads to some "fun" instructions in the Glyphs manual.
- I'm expecting to use:
  - Ubuntu Linux VM
  - FontForge for font dev
  - LibreOffice Writer as test bench

I'm planning to lean heavily on the tutorial
["Creating Fonts with Inkscape and FontForge"](https://www.reddit.com/r/neography/comments/818364/creating_fonts_with_inkscape_and_fontforge_table/).

## Ubuntu Font Management
Make sure you have ~/.local/share/fonts created and fontconfig package
installed.

### Adding
- Drop font files in ~/.local/share/fonts
- Bust cache: `fc-cache -f -v`
- Verify font present: `fc-list | grep FONT`
- Relaunch apps

### Removing
- Delete font files
- Rebuild cache: `fc-cache`

(Source: [random internet](https://linoxide.com/linux-how-to/install-fonts-on-ubuntu/))
