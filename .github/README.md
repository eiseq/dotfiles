<div align=center>
  
![aeondotfiles](https://user-images.githubusercontent.com/123886904/218887856-642bd803-653b-4f06-8db6-0fd1bfa7646c.gif)
  
![](https://img.shields.io/github/last-commit/seeingangelz/dotfiles?&logo=github&style=for-the-badge&color=798ca6&logoColor=D9E0EE&labelColor=191c27)
[![](https://img.shields.io/github/repo-size/seeingangelz/dotfiles?color=798ca6&logo=hackthebox&logoColor=D9E0EE&style=for-the-badge&labelColor=191c27)](https://github.com/seeingangelz/dotfiles)

</div>

<img align="right" src="https://user-images.githubusercontent.com/123886904/227395745-2f3413cb-74fc-4c49-9e92-7774e54f6850.png" alt="Rice Preview" width="363px"/>

```go
❄️                  Setup / DWM                   ❄️
---------------------------------------------------
╭─ Distro          -> Arch Linux
├─ Editor          -> NeoVim / Emacs
├─ Browser         -> Firefox / qutebrowser
├─ Shell           -> zsh
╰─ Process Viewer  -> htop
 
╭─ Music Player    -> cmus
├─ Compositor      -> picom
├─ Notifications   -> dunst
├─ Media Player    -> mpv
╰─ File Manager    -> ranger
 
╭─ WM              -> dwm
├─ Terminal        -> st
├─ App Laucher     -> dmenu
├─ Theme           -> pywal
╰─ Font            -> JetBrainsMono
```
<p align="center">
  <img src="https://user-images.githubusercontent.com/123886904/227397641-517eafd9-3b75-44d1-b3eb-96e839eb4d50.gif" width="500px" alt="DWM Rice"/>
</p>
<br>

> **Warning**
>
> This is my private Arch Linux configuration. It is recommended to use it only for inspiration, as there is no guarantee that it will work for you.
> 
> I am no Arch expert. I'm just a Arch user.
>
<br>

<div align=center>
  
```ocaml
❄️ Installation 魅
```
</div>

<details>
<summary><b>Manual</b></summary>
<br>

> Assuming your **AUR Helper** is [yay](https://github.com/Jguer/yay).

```sh
yay -S cava slop devour exa tty-clock-git picom-animations-git cmatrix-git pipes.sh qt5-styleplugins checkupdates+aur wal-telegram-git webtorrent-cli python-pywalfox arandr arc-gtk-theme clipmenu zsh cmus dbus dunst emacs feh ffmpeg ffmpegthumbnailer firefox flameshot fzf git gnu-free-fonts go htop imagemagick lxappearance mpv neofetch neovim noto-fonts noto-fonts-cjk noto-fonts-emoji numlockx obs-studio openssh perl pulseaudio pulsemixer python-pip python-pywal qalculate-gtk qt5ct qutebrowser ranger syncthing sxiv telegram-desktop tmux tree ttf-jetbrains-mono ttf-nerd-fonts-symbols-common ttf-nerd-fonts-symbols-2048-em-mono ueberzug redshift unzip vim webkit2gtk xclip yt-dlp zathura zathura-pdf-mupdf zip xorg-server xorg-xinit libx11 libxinerama libxft base base-devel
```
```sh
git clone https://github.com/seeingangelz/dotfiles.git
```

> Create [symbolic links](https://www.freecodecamp.org/news/linux-ln-how-to-create-a-symbolic-link-in-linux-example-bash-command/) to the files/directories you need.

</details>

<details>
<summary><b>Automatic</b></summary>
<br>

> Install [git](https://github.com/git/git)

```sh
sudo pacman -Syu git
```
> Clone this repo

```sh
git clone https://github.com/seeingangelz/dotfiles.git
```
> Go to folder

```sh
cd dotfiles/
```
> Give permission to the script

```sh
chmod +x install
```
> Execute the script

```sh
./install
```

</details>
<br>

<div align=center>
  
```ocaml
❄️ Suckless Build お
```
<br>
</div>

<details>
<summary><b>DWM Patches 火</b></summary>
<br>  
<table>
  <tr>
    <td>
      <a href="https://dwm.suckless.org/patches/xresources/">
        <p title="Allows to handle settings from Xresources."><kbd>xresources</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/vanitygaps/">
        <p title="Adds gaps between client windows."><kbd>vanitygaps</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://github.com/bakkeby/patches/blob/master/dwm/dwm-riodraw-nopidmatching-6.2.diff">
        <p title="Provides a resize-by-drawing terminal functionality."><kbd>riodraw</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/preserveonrestart/">
        <p title="Preserves clients on old tags."><kbd>preserveonrestart</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/movestack/">
        <p title="Allows you to move clients around in the stack and swap them with the master."><kbd>movestack</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/exitmenu/">
        <p title="Simple exit menu for dwm."><kbd>exitmenu</kbd></p>
      </a>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://dwm.suckless.org/patches/statuscmd/">
        <p title="This patch adds the ability to signal a status monitor."><kbd>statuscmd</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/statusallmons/">
        <p title="Draws and updates the statusbar on all monitors."><kbd>statusallmons</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/underlinetags/">
        <p title="Underlines selected tags."><kbd>underlinetags</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/swallow/">
        <p title='Adds "window swallowing" to dwm.'><kbd>swallow</kbd></p>
      </a>
    </td>
        <td>
      <a href="https://dwm.suckless.org/patches/pertag/">
        <p title="Keeps layout, mwfact, barpos and nmaster per tag."><kbd>pertag</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/resizecorners/">
        <p title="The mouse is warped to the nearest corner and you resize it from there."><kbd>resizecorners</kbd></p>
      </a>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://dwm.suckless.org/patches/alpha/">
        <p title="Allow dwm to have translucent bars, while keeping all the text on it opaque."><kbd>alpha</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/colorbar/">
        <p title="Lets you change the foreground and background color of every statusbar element."><kbd>colorbar</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/truecenteredtitle/">
        <p title="Center the title with proportion to the area that the title has."><kbd>truecenteredtitle</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/noborder/">
        <p title="Remove the border when there is only one window visible."><kbd>noborder</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/cfacts/">
        <p title="Provides the ability to assign different weights to clients in their respective stack in tiled layout."><kbd>cfacts</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/centeredmaster/">
        <p title="Centers the nmaster area on screen."><kbd>centeredmaster</kbd></p>
      </a>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://dwm.suckless.org/patches/fibonacci/">
        <p title="Adds two new layouts that arranges all windows in Fibonacci tiles."><kbd>fibonacci</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/statusbutton/">
        <p title="Adds a clickable button to the left hand side of the statusbar."><kbd>statusbutton</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://dwm.suckless.org/patches/scratchpads/">
        <p title="Enables multiple scratchpads."><kbd>scratchpads</kbd></p>
      </a>
    </td>
  </tr>
</table>
  
> **Note**
>
> Hover over the patch to receive information about it.
  
</details>
<details>
<summary><b>ST Patches 水</b></summary>
<br>  
<table>
  <tr>
    <td>
      <a href="https://st.suckless.org/patches/xresources/">
        <p title="Adds the ability to configure st via Xresources."><kbd>xresources</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://st.suckless.org/patches/alpha/">
        <p title="Allows users to change the opacity of the background."><kbd>alpha</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://st.suckless.org/patches/boxdraw/">
        <p title="Custom rendering of lines/blocks/braille characters for gapless alignment."><kbd>boxdraw</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://st.suckless.org/patches/scrollback/">
        <p title="Scroll back through terminal output."><kbd>scrollback</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://st.suckless.org/patches/scrollback/st-scrollback-mouse-20220127-2c5edf2.diff">
        <p title="Apply the following patch on top of the previous to allow scrolling using mouse."><kbd>scrollback-mouse</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://st.suckless.org/patches/anysize">
        <p title="Allows st to resize to any pixel size."><kbd>anysize</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://st.suckless.org/patches/workingdir">
        <p title="Allows user to specify the initial path st should use as working directory."><kbd>workingdir</kbd></p>
      </a>
    </td>
  </tr>
</table>

> **Note**
>
> Hover over the patch to receive information about it.
</details>

<details>
<summary><b>DMENU Patches 矢</b></summary>
<br>
<table>
  <tr>
    <td>
      <a href="https://tools.suckless.org/dmenu/patches/center/">
        <p title="Centers dmenu in the middle of the screen."><kbd>center</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://tools.suckless.org/dmenu/patches/border/">
        <p title="Adds a border around the dmenu window."><kbd>border</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://tools.suckless.org/dmenu/patches/password/">
        <p title="Will not directly display the keyboard input."><kbd>password</kbd></p>
      </a>
    </td>
      <td>
      <a href="https://tools.suckless.org/dmenu/patches/alpha/">
        <p title="Adds translucency to the dmenu window, while keeping the text in it opaque."><kbd>alpha</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://tools.suckless.org/dmenu/patches/case-insensitive/">
        <p title="Changes case-insensitive item matching to default behaviour."><kbd>case-insensitive</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://tools.suckless.org/dmenu/patches/highlight/">
        <p title="Highlights the individual characters of matched text for each dmenu list entry."><kbd>highlight</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://tools.suckless.org/dmenu/patches/numbers/">
        <p title="Adds text which displays the number of matched and total items in the top right corner of dmenu."><kbd>numbers</kbd></p>
      </a>
    </td>
    <td>
      <a href="https://tools.suckless.org/dmenu/patches/xresources/">
        <p title="Adds the ability to configure dmenu via Xresources."><kbd>xresources</kbd></p>
      </a>
    </td>
  </tr>
</table>

> **Note**
>
> Hover over the patch to receive information about it.
</details>

<details>
<summary><b>Keybinds 麗</b></summary>
<br>
<i><kbd>Super</kbd> + <kbd>Enter</kbd> = Create a new terminal.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>Q</kbd> = Close a window.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>R</kbd> = Restart DWM.</i><br>
<i><kbd>Super</kbd> + <kbd>LeftArrow</kbd> , <kbd>RightArrow</kbd> = Move to another window.</i><br>
<i><kbd>Super</kbd> + <kbd>M</kbd> = Monocle layout.</i><br>
<i><kbd>Super</kbd> + <kbd>T</kbd> = Tiled layout.</i><br>
<i><kbd>Super</kbd> + <kbd>F</kbd> = Spiral layout.</i><br>
<i><kbd>Super</kbd> + <kbd>U</kbd> = Centered master layout.</i><br>
<i><kbd>Super</kbd> + <kbd>O</kbd> = Grid layout.</i><br>
<i><kbd>Super</kbd> + <kbd>B</kbd> = Toggle the top bar.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>1/4</kbd> = Move a window to another tag.</i><br>
<i><kbd>Super</kbd> + <kbd>1/4</kbd> = Switch to another tag.</i><br>
<i><kbd>Super</kbd> + <kbd>I</kbd> = Increment master.</i><br>
<i><kbd>Super</kbd> + <kbd>D</kbd> = Decrement master.</i><br>
<i><kbd>Super</kbd> + <kbd>H</kbd> = Move mfact to the left.</i><br>
<i><kbd>Super</kbd> + <kbd>L</kbd> = Move mfact to the right.</i><br>
<i><kbd>Super</kbd> + <kbd>K</kbd> = Move cfact down.</i><br>
<i><kbd>Super</kbd> + <kbd>J</kbd> = Move cfact up.</i><br>
<i><kbd>Super</kbd> + <kbd>Space</kbd> = Toggle last layout.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>Space</kbd> = Toggle floating window.</i><br>
<i><kbd>Super</kbd> + <kbd>=</kbd> = Increment gaps.</i><br>
<i><kbd>Super</kbd> + <kbd>-</kbd> = Decrement gaps.</i><br>
<i><kbd>Super</kbd> + <kbd>Alt</kbd> + <kbd>0</kbd> = Restore gaps.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>=</kbd> = Increment vertical gaps.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>-</kbd> = Decrement vertical gaps.</i><br>
<i><kbd>Super</kbd> + <kbd>Control</kbd> + <kbd>=</kbd> = Increment horizontal gaps.</i><br>
<i><kbd>Super</kbd> + <kbd>Control</kbd> + <kbd>-</kbd> = Decrement horizontal gaps.</i><br>
<i><kbd>Super</kbd> + <kbd>Alt</kbd> + <kbd>=</kbd> = Increment inside gaps.</i><br>
<i><kbd>Super</kbd> + <kbd>Alt</kbd> + <kbd>-</kbd> = Decrement inside gaps.</i><br>
<i><kbd>Super</kbd> + <kbd>F1</kbd> = Open file manager.</i><br>
<i><kbd>Super</kbd> + <kbd>F2</kbd> = Open browser.</i><br>
<i><kbd>Super</kbd> + <kbd>F3</kbd> = Open messaging application.</i><br>
<i><kbd>Super</kbd> + <kbd>F4</kbd> = Open music player.</i><br>
<i><kbd>Super</kbd> + <kbd>F5</kbd> = Open code editor.</i><br>
<i><kbd>Super</kbd> + <kbd>F6</kbd> = Open audio manager.</i><br>
<i><kbd>Super</kbd> + <kbd>F7</kbd> = Open screen recorder.</i><br>
<i><kbd>Super</kbd> + <kbd>F11</kbd> = Lockscreen.</i><br>
<i><kbd>Super</kbd> + <kbd>F12</kbd> = Open calculator.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>N</kbd> = Toggle nightmode.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>E</kbd> = Theme selector.</i><br>
<i><kbd>Super</kbd> + <kbd>Control</kbd> + <kbd>E</kbd> = Emoji selector.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>S</kbd> = Manage dotfiles.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>Y</kbd> = Manage clipboard.</i><br>
<i><kbd>Super</kbd> + <kbd>PrtSc</kbd> = Fullscreen screenshot.</i><br>
<i><kbd>PrtSc</kbd> = Screenshot of the selected area.</i><br>
<i><kbd>AudioLowerVolume</kbd> = Volume control down.</i><br>
<i><kbd>AudioRaiseVolume</kbd> = Volume control up.</i><br>
<i><kbd>AudioMute</kbd> = Toggle mute.</i><br>
<i><kbd>Alt</kbd> + <kbd>Z</kbd> = Toggle mute mic.</i><br>
<i><kbd>MonBrightnessUp</kbd> = Increment brightness.</i><br>
<i><kbd>MonBrightnessDown</kbd> = Decrement brightness.</i><br>
<i><kbd>Super</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> = Power Menu.</i><br>
<p title="(Only if it is installed...)"><i><kbd>Super</kbd> + <kbd>P</kbd> = Open DMENU.</p></i>

</details>

<img src="https://user-images.githubusercontent.com/123886904/218294072-d474a330-7464-430a-b369-91f79373dbca.svg" width="100%" title="Footer">
