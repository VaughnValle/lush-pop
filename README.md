# Lush Pop!
A clean and green theme for Pop! OS

## Preview
Love the content? Subscribe to my Youtube Channel: https://tinyurl.com/ydx35uwd 

[![Lush - A Nature Themed Linux Setup](https://github.com/VaughnValle/demo/blob/master/LUSH.png)](http://www.youtube.com/watch?v=URae0PTtJXE "")

## Dependencies
### MNML_Conky
Depends on:
* __git__
* __conky__ ```1.10.x``` (build)
* __curl__ (build)
* __jq__ (build)
* __gawk__ (build)
* __[Conky Vision](https://github.com/zagortenay333/conky-Vision)__ (Conky theme)
* __[OpenWeatherMap](http://openweathermap.org)__ (weather forecast) 
* __[Poiret One](https://fonts.google.com/specimen/Poiret+One)__ (fonts)

### Latte-dock
Depends on (full list [here](https://github.com/KDE/latte-dock#requirements)):
* __Plasma__ ```>= 5.15.```
* __Qt__ ```>= 5.12```

### Lightdm
Depends on:
* __lightdm-webkit2-greeter__
* __[Glorious Lightdm webkit2 theme](https://github.com/manilarome/lightdm-webkit2-theme-glorious)__

## Installation Steps (Ubuntu/Pop! OS 20.04) TODO
1. Update repositories with 

		 sudo apt update
2. Upgrade system with 

		 sudo apt upgrade
3. Install KDE Plasma (desktop only package):

		 sudo apt install kde-plasma-desktop
4. Install Lightdm:

		 sudo apt install lightdm
5. Install Kvantum:

		 sudo apt install qt5-style-kvantum qt5-style-kvantum-themes
6. Install Conky and dependencies:

		 sudo apt install conky-all curl jq gawk
7. Install latte-dock pre-requisites:

		 sudo apt install libxcb-randr0-dev libx11-xcb-dev
8. Shutdown system:

		 sudo shutdown -h now
9. Select KDE Plasma in the DE menu and login
10. Apply the following themes:
* __Global Theme:__ Sweet-Mars
* __Plasma Style:__ ROUNDED
* __Application Style:__ Breeze (_preference_)
* __Window Decorations:__ Sweet Mars-transparent (_preference_)
11. Clone this GitHub repo:

		 git clone https://github.com/VaughnValle/lush-pop.git
12. Apply colorscheme
* Go to __Colors__ in System Settings
* Click on the __Install from file__ button
* Navigate to __lush-pop__ and select __Nature.colors__
* Click __Apply__ to apply colorscheme
13. Install latte-dock extra dependencies (more info [here](https://github.com/KDE/latte-dock/blob/master/INSTALLATION.md_)):

		 sudo apt install cmake extra-cmake-modules qtdeclarative5-dev libqt5x11extras5-dev libkf5iconthemes-dev libkf5plasma-dev libkf5windowsystem-dev libkf5declarative-dev libkf5xmlgui-dev libkf5activities-dev build-essential libxcb-util-dev libkf5wayland-dev git gettext libkf5archive-dev libkf5notifications-dev libxcb-util0-dev libsm-dev libkf5crash-dev libkf5newstuff-dev
