### update package list
sudo pacman -Syy

### update and upgrade all	
sudo pacman -Syu	

### install specific package	
sudo pacman -S pkgname

### find available packages
sudo pacman -Ss keyword	

### find available local packages
sudo pacman -Qs keyword

### list all files from package	
pacman -Ql pkgname

### pacman log file
/var/log/pacman.log

### screen recording
gtk-recordmydesktop

### Mmunt iso file
fuseiso -p  testimage.iso testimagemountpoint

### to unmount
fusermount -u <mountpoint>
  
### to remove a package and its dependencies which are not required by any other installed package
sudo pacman -Rs package_name

### list all packages no longer required as dependencies
sudo pacman -Qdt

### remove all packages no longer required as dependencies
sudo pacman -Rns $(pacman -Qdtq)

### get IP address
ip addr

### update and upgrade yaourt packages
yaourt -Syua

### get distro version
lsb_release -a

### further 
https://devhints.io/pacman