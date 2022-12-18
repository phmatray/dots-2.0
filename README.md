# dots-2.0 - Tuxedo Pulse 15 Gen 2 Edition

## About this fork

In this fork, I've made some changes to the original repo, including:

* Replacing zsh with fish
* Replacing the following applications:
  * Browser: Brave ==> Firefox
  * File manager: Thunar ==> Nautilus
* Cleaning up the code a bit
* Use tctl to get the processor temperature

### Resolutions

* 2560x1440

```
2560
- left and right padding; 2 x 20 = 40  ==> 2520
- left and right bar width; 2 x 600 = 1200  ==> 1320
- left and right bar padding; 2 x 20 = 40  ==> 1280
- center bar width; 1280  ==> 0
```
## An updated, revised version of my dotfiles

Dotfiles for this [post](https://www.reddit.com/r/unixporn/comments/wosl44/bspwm_decided_to_finally_learn_how_to_use_eww/).

<p align="center">
  <img src="https://user-images.githubusercontent.com/98569017/188286072-d91b2027-7fc7-4a65-a45b-223d378afca0.png" width=30% height=30%>
  <img src="https://user-images.githubusercontent.com/98569017/188286092-9131b97a-aa50-4fe8-9179-3cda440c1abc.png" width=30% height=30%>
  <img src="https://user-images.githubusercontent.com/98569017/188286460-d450f8b0-545d-4612-9a8b-99dafe223ed5.png" width=30% height=30%>
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/98569017/188286589-7b0fea41-b8f9-42f8-b376-175a13ef8fd7.gif"
</p>

I started using eww as a bar so I wrote everything from scratch and took the opportunity to be more organized.

For the wallpaper dependant colorschemes use: `.bscripts/wallset <path to wallpaper>`.

The profile picture shown in the lockscreen can be changed by putting the desired image in `~/.face`.

Please note that this rice was made for a single 1080p monitor setup, If you have anything different than that you'll have to tweak some things on your own.

The picom fork used for animations might be a little unstable. For any graphical glitches you may be having, toggle it off and on again with `super+p`

## Dependency list:
### AUR packages
Just run this for this section (assuming you use yay):
```
yay -Sy acpi alsa-utils-git blueman firefox bspwm colorpicker dunst eww-git flameshot hsetroot imagemagick jq kitty mantablockscreen network-manager-applet pa-applet-git picom-animations-git playerctl polkit-gnome polybar pulseaudio python3 rofi scrot sox spicetify-cli spotify sxhkd thunar wmctrl wpgtk-git xclip xdotool xprintidle xwinfo-git --needed
```
If you're not using arch, this is the dependency list, install in wathever way you want:
- acpi
- alsa-utils
- blueman
- firefox
- bspwm
- colorpicker
- dunst
- eww
- flameshot
- hsetroot
- imagemagick
- jq
- kitty
- mantablockscreen
- network-manager-appler
- pa-applet
- picom-animations-git
- playerctl
- polkit-gnome
- polybar
- pulseaudio
- python3
- rofi
- scrot
- sox
- spicetify-cli
- spotify
- sxhkd
- thunar
- wmctrl
- wpgtk
- xclip
- xdotool
- xprintidle
- xwinfo

### Other
- [brightlight](https://github.com/multiplexd/brightlight) since for some reason xbacklight doesn't work on my machine. It's only used in `.bscripts/brightness.sh` so feel free to edit that script if you wanna use xbacklight instead.
- [pop_report](https://github.com/ikz87/pop_report) used in some scripts.

### Optional
- plasma-integration [AUR package](https://aur.archlinux.org/packages/plasma-integration-git) and [chrome extension](https://chrome.google.com/webstore/detail/plasma-integration/cimiefiiaegbelhefglklhhakcgmhkai/related?hl=es) to better integrate media playing in brave with widgets (like having thumbnails of youtube videos show up in the left bar).


Please let me know if any packages are still missing.

## Installing
just run install.sh:
```
chmod +x install.sh
./install.sh
```

TODO: Add a keybinds guide, you can read about keybinds in .config/bspwm/sxhkdrc for now.
