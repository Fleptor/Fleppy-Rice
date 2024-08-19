==Fleppy's Rice===
Fleptor's rice of the dwm window manager.

Ricing is a the process of customising visual aspects of the operating system based on user perference,
and the Dynamic Window Manager (stylized: dwm) is Suckless's own window manager, built with philosophy
of less is more, and one mustn't learn an additional scripting language just to configure it.

And for someone like me who prefers simplicity and minimalism, dwm is quite the dream when it comes
to window managers, but I'm no C expert, and to patch dwm you have to edit the source code directly,
and luckily the amazing suckless community had provided us with many great useful and quality of life
patches which we could add to dwm's source code.

And to save myself the hassle of having to set it up manually everytime and remembering which packages
to install alongside the rice, I've neatily gathered them up in one git repository.

|=========================================================================|
|============================= KEYBINDS LIST =============================|
|=========================================================================|
 * MOD KEY: The super key, aka the windows key, aka meta key.
 -- Crucial keybinds: 
 Open terminal(st):          MOD + RETURN.
 Close window:               MOD + Shift + Q.
 Open dmenu:                 MOD + P.
 Switch to tags from 1 to 9: MOD + (1 to 9).
 Move window to tags 1 to 9: MOD + Shift + (1 + 9).
 Restart dwm:                Ctrl + MOD + Shift + Q.
 Exit dwm:                   MOD + Shift + Delete.

 -- Window manipulation:
 Switch focus to next window:     MOD + J.
 Switch focus to previous window: MOD + K.
 Increase focused window width:   MOD + L.
 Decrease focused window width:   MOD + H.
 Move focused window in stack:    MOD + Shift + (J or K). 
 Switch to floating layout:       MOD + Shift + F or MOD + Space.
 Switch to tiling layout:         MOD + Shift + T.
 Switch to monocle layout         MOD + Shift + M.
 Toggle fullscreen on a window:   MOD + F.
 Set window to floating mode:     MOD + Shift + Space.
 Center a floating window:        MOD + C.
 Show all open windows:           MOD + 0.
 Pin window to all tags:          MOD + Shift + 0.
 Tile windows vertically:         Mod + D (To revert, do MOD + I).

 -- Gaps:
 Increase gap margins: MOD + Plus.
 Decrease gap margins: MOD + Minus.
 Disable gaps:         MOD + Shift + Plus.
 Reset gap margins:    MOD + Shift + Minus.

 -- Extra functionality:
 Move focus between windows: Alt + Tab.
 Take screenshots: prtScr (Print Screen Key).
 Go back and forth between current and last tag: MOD + V.
 Open Firefox: MOD + R.
 Toggle bar:   MOD + B.

|=========================================================================|
|=============================PATCHES APPLIED=============================|
|=========================================================================|
- Patches applied to dwm:
 1) Functional Gaps.
 2) Per Tag.
 3) Actuall Fullscreen.
 4) Restart DWM.
 5) Alt Tab.
 6) Auto Start.
 7) Center Window Keybind.
 8) Bar Padding.
 9) Move Stack.

- Patches applied to dmenu:
 1) Center.
 2) Border.
 3) Numbers.

|=========================================================================|
|=============================PACKAGES NEEDED=============================|
|=========================================================================|
 1) feh
 2) picom
 3) JetbrainsMono
 4) fontawesome
 5) flameshot
 6) xkblayout-state (AUR)

|=========================================================================|
|=============================INSTRUCTIONS================================|
|=========================================================================|
 1) Clone repo and compile dwm, dmenu and dwmblocks (with make clean install).

 2) Move DWM.desktop file to /usr/share/xsessions to access dwm from the
    display manager, or via xinit if you fancy that.

 3) Create an autoastart file at ~/.dwm/ directory to include script and/or
    other utilities desired to be started alongside dwm.

 4) Install the above listed packages. 

 5) To display wallpapers, check out feh.

 6) Current terminal emulator is set to st, to change it, in config.h
    file, edit line 88. 
