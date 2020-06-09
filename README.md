# rofi-vim
A Vim cheat sheet for Rofi

I wanted to create a quick searchable Vim cheat sheet, and I decided to use a
text file as the cheat sheet and then pipe that to a Rofi dmenu.

## Example
If you have Rofi installed you can try it out like this:

```bash
curl -s https://raw.githubusercontent.com/rdvm/rofi-vim/master/vimcheat | rofi -dmenu -i -font "mono 20" -columns 2 -width 100 -location 1 -lines 20 -bw 2 -yoffset -2
```

Or if you have dmenu installed:

```bash
curl -s https://raw.githubusercontent.com/rdvm/rofi-vim/master/vimcheat | dmenu -i -l 30
```

## Instuctions

The `rofi-vim` file in this repository is the script I use on my system to
launch the cheat sheet. The structure of the script was copied from [this
gist](https://gist.github.com/tadly/0741821d3694deaec1ee454a95c591fa) created
by [tadly](https://gist.github.com/tadly) for using Rofi as an emoji picker.
:grinning:

The script will download the cheat sheet file from this repo and cache it
locally so it only needs to be downloaded once. You can also use the
``--download`` argument to refresh the cheat sheet in case it's changed.
