# Lush Pop!
A clean and green theme for Pop! OS

## Preview
Love the content? Consider Subscribing: https://tinyurl.com/ydx35uwd 

[![Lush - A Nature Themed Linux Setup](https://github.com/VaughnValle/demo/blob/master/fus.png)](http://www.youtube.com/watch?v=dQ1yh-UtfuE)

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
__NOTE:__ Replace ```$DIR``` with the directory you cloned this repo to 

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
    - __Global Theme:__ Sweet-Mars
    - __Plasma Style:__ ROUNDED
    - __Application Style:__ Breeze (_preference_)
    - __Window Decorations:__ Sweet Mars-transparent (_preference_)
11. Clone this GitHub repo:

		 git clone https://github.com/VaughnValle/lush-pop.git
12. Apply colorscheme
    - Go to __Colors__ in System Settings
    - Click on the __Install from file__ button
    - Navigate to __lush-pop__ and select __Nature.colors__
    - Click __Apply__ to apply colorscheme
13. Install latte-dock extra dependencies (more info [here](https://github.com/KDE/latte-dock/blob/master/INSTALLATION.md_)):

		 sudo apt install cmake extra-cmake-modules qtdeclarative5-dev libqt5x11extras5-dev libkf5iconthemes-dev libkf5plasma-dev libkf5windowsystem-dev libkf5declarative-dev libkf5xmlgui-dev libkf5activities-dev build-essential libxcb-util-dev libkf5wayland-dev git gettext libkf5archive-dev libkf5notifications-dev libxcb-util0-dev libsm-dev libkf5crash-dev libkf5newstuff-dev
14. Install latte-dock with the installation script:

		 cd $DIR/lush-pop/latte-dock && sh install.sh
15. Launch latte-dock either in __Krunner__ (alt+space) or in the terminal with:

		 latte-dock
16. Switch to __Extended__ layout
    - Right click the dock, 
    - Click __Configure Latte__
    - Switching the layout in the __Layouts__ section
17. Adjust the latte-dock settings to your liking
    - Right click the dock
    - Click __Edit Panel__
    - Toggle the __Advanced__ option
18. Remove/Add your preferred widgets, widgets in the video includes:
    - __Global Menu__
    - __Application Title__
    - __Better Inline Clock__
19. Configure __System Tray__ and set all menus to __Always hidden__
20. Arrange widgets to your liking
    - You can enable colors in your widget by clicking the __teardrop icon__ 
21. Configure the __Better Inline Clock__ widget
22. Adjust the padding of the dock 
    - In the __Effects__ section of the latte-dock settings, adjust the _Padding_ slider
23. Configure __Application Launcher__ icon
    - Sample icon is in ```$DIR/lush-pop/``` as __icon.png__
24. Configure Kvantum Manager and set the theme
    - Sweet Mars Kvantum theme folder is in ```$DIR/lush-pop/Sweet-Mars-transparent-toolbar```
25. Create a free account in [OpenWeatherMap](https://openweathermap.org/) 
    - Get your free API key in the __API__ section of the website
    - Search the City ID of your location
26. Install the Poiret One font in ```$DIR/lush-pop/Poiret```
27. Install MNML Conky:

		 cd $DIR/lush-pop/mnml_conky && ./install
    - __NOTE__: Leave your answers blank when prompted during installation by hitting __Enter__
28. Copy conky configuration file to your home directory:

		 cp .conkyrc ~/.conkyrc
29. Edit the conky configuration file:

		 nano ~/.conkyrc
30.     - Place your __API key__ in the ```template6``` variable
        - Place your __City ID__ in the ```template7``` variable
31. Run conky in the terminal:

		 conky
32. Install Kwin Scripts:
    - __Krohnkite__ for window-tiling
    - __Latte Window Colors__ for better dynamic latte-dock colors
33. Remove top titlebar of terminal windows
    - Open the __Window Rules__ setting
    - Change __Window Class__ type to __Exact Match__ and type in your terminal (e.g. Konsole)
    - Tick the __No titlebar and Frame__ setting in the _Appearance section_, select __Force__ and __Yes__
34. Enable Configuration settings for Krohnkite:

		 mkdir -p ~/.local/share/kservices5/
		 ln -s ~/.local/share/kwin/scripts/krohnkite/metadata.desktop ~/.local/share/kservices5/krohnkite.desktop
35. Configure Krohnkite in 
    - __Kwin Scripts__ for visuals such as window gaps, tiling modes, etc.
    - __Global Shortcuts__ _Kwin_ section for Krohnkite shortcuts
36. Change your terminal theme to your liking
    - Theme used in the video is __Sweet Mars__, included in the __Sweet Konsole Theme__
37. Install the custom splash screen with 

		 cd $DIR/lush-pop/ && cp -r Lush ~/.local/share/plasma/look-and-feel/
38. Preview and apply the installed custom splash screen
    - Go to __Splash Screen__ settings
    - Find the __Lush__ splash screen; hit the play button to preview
    - Select __Lush__ and hit apply
39. Install lightdm-webkit2-greeter
    - Open Dolphin in $DIR/lush-pop
    - Install the __lightdm-webkit2-greeter_2.2.5-1%2B15.31_amd64.deb__ file; you can use __Eddy__
40. Install the __Glorious__ Webkit2 theme:

		 sudo cp -r $DIR/lush-pop/lightdm-webkit2-theme-glorious/ /usr/share/lightdm-webkit/themes/
41. Edit the lightdm configuration file:

		 sudo nano /etc/lightdm/lightdm.conf.d/lightdm.conf
    - Change the value of __greeter-session__ to ```lightdm-webkit2-greeter```
42. Edit the lightdm webkit2 configuration file:
		 sudo nano /etc/lightdm/lightdm-webkit2-greeter.conf
    - Change the value of __webkit_theme__ to ```lightdm-webkit2-theme-glorious```
43. Reboot your system and enjoy!
