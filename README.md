# troubleshoot
I'm tired of fixing the same problem over and over again. 

## Linux 

### RDP (Gnome Remote Desktop)

- In case you're trying to connect to gnome with remote desktop (windows -> gnome) and the screen is blank, try this:
  - https://discourse.gnome.org/t/how-to-configure-connect-to-the-new-headless-gnome-remote-desktop-service/19634/12

### Authentication (Fingerprint)

- In case the fingerprint option does not show up in GNOME
  - https://discussion.fedoraproject.org/t/fingerprint-reader-does-not-work/104739/3

### Mesa Drivers (AMD)  
- KDE: In case screen is going black while in fullscreen, try disabling Adaptative Sync
  - https://discussion.fedoraproject.org/t/fedora-40-nvidia-gpu-wayland-intermittent-black-screen-with-full-screen-applications/130770/7

### Godot

- In case godot is not opening using nvidia gpu, this can help:
  - https://forum.godotengine.org/t/unable-to-use-nvidia-gpu-with-godot-4-3-under-linux/80124/6
 
### Emacs

- Doom emacs is not loading on startup
  - https://github.com/doomemacs/doomemacs/issues/7292#issuecomment-1630204067

## Windows

### SSH
- Git clone hangs on receiving objects or any other ssh operation
  - This fixes it: https://stackoverflow.com/a/79075865
 
## Tooling

### EditorConfig
- If you ever bumped in a situation where your editor keeps adding newline after you edit a markdown file, it may be because of this https://stackoverflow.com/a/67752027

### VSCode
- VSCode remote development hangs with ssh timeout: https://stackoverflow.com/a/62038186

### SSH
- To log-in to that server configured in .ssh/config, one must add this to their `.bashrc[_logout]` in order to auto `ssh-add`
  - https://unix.stackexchange.com/a/90869
