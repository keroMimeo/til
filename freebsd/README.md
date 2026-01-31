## FreeBSD command line

```bash


// show the desktop environments on the system
> bectl list

// update the OS and kernel
freebsd-update fetch
freebsd-update install
pkg update && pkg upgrade



```


## Applications to install

- [x] Firefox  
  sudo pkg install 

- [x] Git  
  sudo pkg install git  

- [x] Visual studio code  
  sudo pkg install vscode

- [x] Chrome
  sudo pkd install chromium

 - [ ] Minecraft

On FreeBSD you need to install something like Prism Launcher.
  pkg install prismlauncher

Java runtime
  pkg install openjdk17

Audio and input
  sudo pkg install openal-soft sdl2


After launching "Prism Launcher" go to Settings/Java and ensure the path points to the correct OpenJDK version.  This is usually at /usr/local/openjdk17/bin/java.  Make sure that "use system installation of LWJGL" is selected.  



Install graphics drivers  
  sudo pkg install drm-kmod  
  
Enable graphics driver at boot:  
  add **lkd_list='i915kms'** to /etc/rc.conf

Ensure your user is in the Video group
  pw groupmod video -m <username>
  pw groupmod render -m <username>











### Configuration  






Terminal / General  

cursor shape = underline;  select 'cursor blinks'  
colors:   background = black;  text = green  

Settings / Mouse & Trackpad  
Devices/Trackpad - disable touchpad while typing  
tap touchpad to click  




