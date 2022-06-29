# kitty-mpd-background
### Automatically change the kitty background to the currently playing song!

install the dependencies by running

`sudo pacman -S kitty mpc ffmpeg`

## To use with ncmpcpp simply run

`curl https://raw.githubusercontent.com/uwulily/kitty-mpd-background/main/change-background > .config/ncmpcpp/change-background & curl https://raw.githubusercontent.com/uwulily/kitty-mpd-background/main/wrapper > .config/ncmpcpp/wrapper`

and add

`execute_on_song_change="~/.config/ncmpcpp/wrapper""`

to your ncmpcpp config

beware this implementation is kinda junky, because i wasnt able to set the background image correctly everytime if the process wasnt detached from the main one
if you know how to fix this/have a better implementation feel free to commit !
