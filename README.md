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
kth-blue = 25,84,166
kth-red = 157,16,45
kth-green = 98,146,46
kth-lightblue = 36,160,216
kth-lightred = 228,54,62
kth-lightgreen = 176,210,43
kth-pink = 216,84,151
kth-yellow = 250,185,25
kth-darkgray = 101,101,108
kth-middlegray = 189,188,188
kth-lightgray = 227,229,227
```
according to the KTH color profile palette
![kth palette](https://intra.kth.se/polopoly_fs/1.486828!/image/fargreferens_png.png)

## Using even better
There is some logic embedded in the package: if you add the name of a dvips color as an option, the package will overwrite that color with the corresponding KTH template color. For instance, running
```
\usepackage[red,blue]{kthcolors}
```
will change all references to the color blue with references to `kth-blue` and all references to the color red to `kth-red`. You can use the flag `all` to change standard colors to their closest KTH matches:
```
blue -> kth-blue
red -> kth-red
green -> kth-green
pink -> kth-pink
yellow -> kth-yellow
gray -> kth-darkgray
```

## Hacking
If you have comments or hacks that you would like to include, send me a message or post an issue or a pull request. Have fun!
