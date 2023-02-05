# kitty-mpd-background
![image showcasing the functionality](https://github.com/lzgirlcat/kitty-mpd-background/blob/main/images/1.png?raw=true)
### Automatically change the kitty background to the currently playing song!

install the dependencies by running

`sudo pacman -S kitty mpc ffmpeg`

## To use with ncmpcpp simply run

`curl https://raw.githubusercontent.com/lzgirlcat/kitty-mpd-background/main/change-background > ~/.config/ncmpcpp/change-background & curl https://raw.githubusercontent.com/lzgirlcat/kitty-mpd-background/main/wrapper > ~/.config/ncmpcpp/wrapper`

and add then

`echo execute_on_song_change="~/.config/ncmpcpp/wrapper" >> ~/.config/ncmpcpp/config`

to your ncmpcpp config

to start ncmpcpp now just run

`kitty -o allow_remote_control=yes --listen-on unix:/tmp/kittyncmpcpp -e ncmpcpp`

beware this implementation is kinda junky, because i wasnt able to set the background image correctly everytime if the process wasnt detached from the main one
if you know how to fix this/have a better implementation feel free to commit !
