This fork uses the original images from macOS instead of the modified ones from the original. I got the original HEIC from a macOS Catalina installation and ran `convert 'Catalina Day.heic' out.png` to convert them into PNGs (the original HEIC isn't compatible with the KDE dynamic wallpaper plugin).

Unlike the project this was forked from, this only works on KDE since I have no idea how the Gnome system works.

# Installation (Arch/Manjaro)

1. Install plasma5-wallpapers-dynamic (`yay -S plasma5-wallpapers-dynamic`)
2. Download wallpaper.heic (feel free to rename it) and place it somewhere
3. Right click on your desktop and click "Configure Desktop..."
4. Set the wallpaper type to dynamic
5. Click on "Add Wallpaper..."
6. Select wallpaper.heic (or whatever you called it)

(btw I'm keeping the old catalina-solar.json because if I ever bother to add a solar config, I'll probably want to use it as a baseline)

# Making your own HEIC

If you want to modify how the wallpaper works, you will need to make your own HEIC. To do this, do this:

1. Clone this repo (`git clone https://github.com/UnicornsOnLSD/gnome-kde-dynamic-wallpaper-catalina.git`)
2. Move metadata.json into original-images
3. Open a terminal in original-images
4. `Run kdynamicwallpaperbuilder metadata.json`
5. Set the generated HEIC as your wallpaper
