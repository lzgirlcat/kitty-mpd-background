# kitty-mpd-background
### Automatically change the kitty background to the currently playing song!

install the dependencies by running

`sudo pacman -S kitty mpc ffmpeg`

## To use with ncmpcpp simply run

`curl https://raw.githubusercontent.com/uwulily/kitty-mpd-background/main/change-background > .config/ncmpcpp/change-background`

and add

`execute_on_song_change="~/.config/ncmpcpp/change-background"`

to your ncmpcpp config
