# FreeBSD

# ZSH
.zshrc
PS1='%n@%m %~$ '

# zsh history
HISTFILE=~/.zsh_history
HISTSIZE=10000
SAVEHIST=10000
setopt appendhistory

# rc.conf
dbus_enable="YES"
xdm_enable="YES"

# wheel
pw group mod wheel -m user

# upgrade
pkg upgrade
 
# /boot/loader.conf
efi_max_resolution="1024x768"
1600x900

mouse problem
ums_load="YES"

# .xinitrc
exec fvwm & setxkbmap -layout fr -variant mac -option "terminate:ctrl_alt_bksp" & xterm & xclock

setxkbmap -layout fr -variant mac -option "terminate:ctrl_alt_bksp"
exec openbox-session

# vmware share : 

/boot/loader.conf
fusefs_load="YES"

/etc/fstab
.host:/    /mnt/hgfs        vmhgfs-fuse    failok,rw,allow_other,mountprog=/usr/local/bin/vmhgfs-fuse   0    0

# sound

/boot/loader.conf
snd_hda_load="YES"

# doas

/etc/doas.conf
permit nopass :wheel

