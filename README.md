# rofi-vim
## A Vim cheat sheet for _Rofi_ or _dmenu_

I wanted to create a quick searchable Vim cheat sheet, and I decided to use a
text file as the cheat sheet and then pipe that to a Rofi dmenu.

## Example
If you have _Rofi_ installed you can try it out like this:

```bash
curl -s https://raw.githubusercontent.com/rdvm/rofi-vim/master/vimcheat | rofi -dmenu -i -font "mono 20" -columns 2 -width 100 -location 1 -lines 20 -bw 2 -yoffset -2
```

Or if you have _dmenu_ installed:

```bash
curl -s https://raw.githubusercontent.com/rdvm/rofi-vim/master/vimcheat | dmenu -i -l 30
```

## Instuctions

The `rofi-vim` file in this repository is the script I use on my system to
launch the cheat sheet. The structure of the script was copied from [this
gist](https://gist.github.com/tadly/0741821d3694deaec1ee454a95c591fa) created
by [**@tadly**](https://github.com/tadly) for using _Rofi_ as an emoji picker.
:grinning:

You can place the script somewhere in the `$PATH` on your system to be able to
call it from anywhere or by using a key-binding.

The script will download the cheat sheet file from this repo and cache it
locally so it only needs to be downloaded once. You can also use the
``--download`` argument to refresh the cheat sheet in case it's changed. When
you run `rofi-vim` it will automatically fetch a fresh copy if the current
cached copy is more than 5 days old.

### Using with _Rofi_ and _dmenu_
There is an optional `--dvim` argument if you want to use _dmenu_ instead of
_Rofi_, and if no argument is supplied it will use _Rofi_ by default.
