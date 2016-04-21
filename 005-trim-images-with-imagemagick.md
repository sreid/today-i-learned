# Trim Images with ImageMagick
Need to cleanup images that have a small border on them? Use the always trusty ImageMagick suite of tools. The ```-shave``` option for ```convert``` works nicely:

```
convert input.png -shave 2x2 output.png
```


Hat tip: https://stackoverflow.com/questions/12200763/imagemagick-chop-30px-off-each-edge-variable-width-and-height
