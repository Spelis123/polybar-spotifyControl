# polybar-spotifyControl
Control Spotify playback from polybar! based off of Jvanrhijn but SUPER UPGRADED :)
[original](https://github.com/Jvanrhijn/polybar-spotify)

Add this to `config.ini`
```
[module/spotify]
type = custom/script
interval = 1
format-prefix = ""
format = <label>
exec = python $HOME/.config/polybar/spotify_status.py -f '{song}'
format-underline = ${colors.background-alt}
click-left = playerctl --player=spotify play-pause
click-right = playerctl --player=spotify next
click-middle = spotify
scroll-up = playerctl position 5+
scroll-down = playerctl position 5-
```
