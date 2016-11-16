# kthcolors
KTH Colorscheme for LaTeX!

## Installing
Make the style file available to your latex distribution.

## Using
It's just a matter of adding
```
\usepackage{kthcolors}
```
to the header of your document (This will also include the `xcolor` package).

The default package provides the following colors from the KTH official color profile:
```
kth_blue = 25,84,166
kth_red = 157,16,45
kth_green = 98,146,46
kth_light_blue = 36,160,216
kth_light_green = 176,210,43
kth_pink = 216,84,151
kth_light_red = 228,54,62
kth_yellow = 250,185,25
kth_dark_gray = 101,101,108
kth_gray = 189,188,188
kth_light_gray = 227,229,227
```
according to the KTH color profile palette
![kth palette](https://intra.kth.se/polopoly_fs/1.486828!/image/fargreferens_png.png)

## Using even better
There is some logic embedded in the package: if you add the name of a dvips color as an option, the package will overwrite that color with the corresponding KTH template color. For instance, running
```
\usepackage[red,blue]{kthcolors}
```
will change all references to the color blue with references to `kth_blue` and all references to the color red to `kth_red`. You can use the flag `all` to change standard colors to their closest KTH matches:
```
blue -> kth_blue
red -> kth_red
green -> kth_green
pink -> kth_pink
yellow -> kth_yellow
gray -> kth_dark_gray
lightblue -> kth_light_blue
lightred -> kth_light_red
lightgreen -> kth_light_green
lightgray -> kth_light_gray
middlegray -> kth_gray
```

## Hacking
If you have comments or hacks that you would like to include, send me a message or post an issue or a pull request. Have fun!
