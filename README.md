# Catbots-All-In-One-Install
## Installation
Open console and paste this:
```dep=""; [ ! -x $(command -v npm) ] && dep="npm $dep"; [ ! -x $(command -v firejail) ] && dep="firejail $dep"; [ ! -x $(command -v route) ] && dep="net-tools $dep"; [ ! -x $(command -v xhost) ] && dep="xorg-xhost $dep"; [ $dep != ""] && sudo pacman -S $dep && git clone https://github.com/nullworks/catbot-setup && cd catbot-setup && bash <(wget -qO- https://raw.githubusercontent.com/nullworks/One-in-all-cathook-install/master/install-all) && ./install-catbots && cd ~/.steam/steam/steamapps/common/Team\ Fortress\ 2/tf/maps && git clone --recursive https://github.com/nullworks/catbot-database && sudo chmod 755 -R . && mv catbot-database/nav\ meshes/* . && rm -rf catbot-database && cd - && git clone https://github.com/TrulyFalseHonesty/convertjs && mv convertjs/convert.js convert.js && rm -rf convertjs && echo username:password >> accounts.js && echo EnJoY HaX Ya LiL CaT!```
## Cathook
To use the cheat, all you have to do is run:
```sudo ./attach```
## Catbots
The bots are a trickier to use, you first need a list of steam accounts.
Put them on the accounts.js file following the username:password format.
type ```./start``` to start the bots and ```./stop``` to stop them.
