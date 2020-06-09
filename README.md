# rofi-vim
A Vim cheat sheet for Rofi

I wanted to create a quick searchable Vim cheat sheet, and I decided to use a
text file as the cheat sheet and then pipe that to a Rofi dmenu.

## Instructions
If you have Rofi installed you can try it out like this:

```bash
curl -s https://raw.githubusercontent.com/rdvm/rofi-vim/master/vimcheat | rofi -dmenu -i -font "mono 20" -columns 2 -width 100 -location 1 -lines 20 -bw 2 -yoffset -2
```

Or if you have dmenu installed:

```bash
curl -s https://raw.githubusercontent.com/rdvm/rofi-vim/master/vimcheat | dmenu -i -l 30
```
