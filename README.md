# Setup
This started as a place to keep my dotfiles but I keep repeating a lot of configuration setup that now it's expanded to more than just that.

## Setting up i3
* Install i3 `sudo apt-get install i3`
* Install lxappearance `sudo apt-get install lxappearance`
* Install compton `sudo apt-get install compton`
* Install feh `sudo apt-get install feh`
* Install rofi `sudo apt-get install rofi`
### Set up fonts
* Create fonts directory `mkdir ~/.fonts`
* Copy fonts `cp -R i3/fonts ~/.fonts`
* Launch lxappearance and set font to SFNS Display
### Set Arc Theme
* Google arc-theme and install for gtk
* Google arc-theme and install for firefox

### Setup i3
* Copy i3config file. `scp i3/config ~/.config/i3/config`
* Copy compton config file `scp i3/compton.conf ~/.config/i3`
* Copy rofi config `mkdir ~/.config/rofi && scp rofi/config ~/.config/rofi`
* Install i3pystatus `https://github.com/enkore/i3pystatus`
* Set the feh background to an appropriate wallpaper

#### Depracated
* Install i3blocks `sudo apt-get install i3blocks`
* Copy i3blocks file. `scp i3/i3blocks.conf ~/.config/i3`

### Other apps to install
* Thunar for file system
* pavucontrol for audio/output devices
** Note: On the dell xps, in order to reset the sound card, you can do `sudo modprobe snd-soc-rt286`

## Setting up VIM
* VIM uses vundle so install that first  `git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim`
* Taskwiki doesn't have markdown features in the main branch so we clone from the special branch: `git clone -b extra-syntaxes https://github.com/DancingQuanta/taskwiki.git ~/.vim/bundle`
* Copy the vimrc `scp vim/.vimrc ~/.vimrc`
* Start up VIM and run `:PluginInstall`

## Setting up Terminal
* Install termite: `sudo apt-get install termite`
* It's already configured as default for i3 in the config
* Install powerline fonts: `https://github.com/powerline/fonts`
* Copy termite config so it looks nice: `mkdir ~/.config/termite && scp termite/config ~/.config/termite/config`

### Gnome terminal (old)
* Get solarized gnome terminal colors from `https://github.com/Anthony25/gnome-terminal-colors-solarized`
