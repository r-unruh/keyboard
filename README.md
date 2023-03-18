# keyboard

xkb keyboard layout for developers that require German umlauts.

## Core aspects
* Uses the US keyboard layout as a base
* Supports German Umlauts and Czech letters (and probably some other languages
  too)
* Uses Capslock as Ctrl-Alt
* Embraces Linux Console Command shortcuts. Examples:
  * Capslock + j simulates Return
  * Capslock + h deletes a character

## Reasoning
I created this keyboard layout in order to replace the default German layout,
which is very impractical for programming.
Since I don't believe constantly switching from US to DE and back is a viable
solution I made this custom layout that allows me to use all the bracket keys
in a reasonable manner as well as typing all German umlauts (and even the
capital ẞ, which is a (newish) part of the German language but the normal German
keyboard layout doesn't have).

## Drawbacks
* You lose the expected functionality of your Capslock key and can't easily
  scream at people in chat anymore
* Takes a while to get used to
* You will have a hard time using normal keyboard layouts afterwards

## Key setup
Please refer to the comments in [rukb](rukb). They should tell you everything
you need to know.

### Installing
Download [rukb](rukb) to your xkb/symbols folder, e.g.:
```
sudo wget -P /usr/share/X11/xkb/symbols https://github.com/r-unruh/keyboard/raw/master/rukb

```
Make sure it is downloaded under the correct file name - especially if you're
updating the layout.

Enable it:
```
setxkbmap rukb
```

To make the change permanent, add `setxkbmap rbkb` to a script that launches
with your X-session.


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file
for details.
