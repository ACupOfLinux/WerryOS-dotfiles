# WerryOS Dotfiles 

This Build of Fedora-Titus is for my project WerryOS where you get to build your own fedora system from the ground up. 

This is the fedora iso you need: https://download.fedoraproject.org/pub/fedora/linux/releases/36/Server/x86_64/iso/Fedora-Server-netinst-x86_64-36-1.5.iso

Be sure to check me out on youtube!! : https://www.youtube.com/channel/UCbyfsrFv9eWJe69iBPZmTLw

these are the commands to install things that you need :)

#Commands:

sudo dnf update -y; sudo dnf install  bspwm -y; sudo dnf install mangohud -y; sudo dnf install picom -y; sudo dnf install kitty; sudo dnf install vim- y; sudo dnf install gimp -y; sudo dnf install sddm -y; sudo dnf install lxpolkit -y; sudo dnf install rofi -y; sudo dnf install polybar -y; sudo dnf install nitrogen -y; sudo dnf install thunar -y;

AUDIO IS SOMETHING YOU NEED TO SETUP YOURSELF!!!!!

#Command list 2
sudo dnf install fontawesome-fonts fontawesome-fonts-web -y 
sudo wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/FiraCode.zip
sudo wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/Meslo.zip
sudo unzip Meslo.zip -d /usr/share/fonts
sudo unzip FiraCode.zip -d /usr/share/fonts

#refresh fonts 
fc-cache -vf

#remove font zips 
rm ./FiraCode.zip ./Meslo.zip

# set Sddm to start on default runlevel 
sudo systemctl enable sddm
sudo systemctl set-default graphical.target

Do all of this as a normal user!

IMPORTANT!!! If you do not know how to install these dotfiles yourself put all of the contents of the dotconfig folder from the git to ~/.config and move .Xnord, .xintitrc, and .Xresources to your home directory 

#optional if you get an X cursor install the xsetroot package with sudo dnf install -y xsetroot

#Optional install xfce to fallback on 

it only takes one simple command! sudo dnf group install "Xfce Desktop"

and that should install everything!!! have fun :)
