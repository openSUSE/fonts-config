fonts-config

------

The source for openSUSE's system fontconfig configurations.

* 10-group-tt-hinted-fonts.conf
* 10-group-tt-non-hinted-fonts.conf
* 13-selective-rendering.conf
* 61-wine-aliases.conf

are from `infinality` project and MIT licensed. 

As the infinality project is officialy dead, we just copied them here
instead of generating it every time.

## Layout

00-09 extra font directories
10-19 system rendering defaults (antialising etc)
20-29 font rendering options
30-39 family substitution
40-49 map family to generic type
50-59 load alternate config files
60-69 generic aliases, map generic to family
70-79 adjust which fonts are available
80-89 match target scan (modify scanned patterns)
90-99 font synthesis

## Debug

[FC_DEBUG](https://www.freedesktop.org/software/fontconfig/fontconfig-user.html#DEBUG) is your friend.

`fc-match -a sans-serif | head -n 10` is also a good command

[EmojiOne Color Font Full Demo](https://eosrei.github.io/emojione-color-font/full-demo.html) is a good place for testing emojis.
