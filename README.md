Better wallpaper widget for qtile

The window manager qtile has a built-in widget called wallpaper. It's working but not very good.
1. It cannot update wallpaper based on certain time like 600 seconds.
2. It cannot filter correct file type so I have to delete all the none image files in the wallpaper folder.
3. It cannot find wallpaper recursively. So my wallpaper in sub-folders cannot be shown.

In order to solve it, thus I made a little adjustment to it.

How to install:
1. Copy wallpaperng.py to ~/.config/qtile
2. In your config.py, import wallpaperng
3. In your widget section,
    wallpaperng.Wallpaperng(**base(bg='color1'), label='', random_selection = True, update_interval=60),
