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
* __Application Style:__ Breeze (preference)
* __Window Decorations:__ Sweet Mars-transparent (preference)
