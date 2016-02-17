<h1>Some routines  in R</h1>

<h2>Quit</h2>

```r
# Use q()
# You will be asked whether to save the image (whole environment).
# It is better to explicitly save what you want (see below).
q()
```
<h2>Save</h2>

```r
# Command history (all commands typed)
savehistory('myhistory.txt')
# An object of interest
save(list_of_object, file='myobject.Robject')
# All objects (the whole environment), 
# also called an image or a snapshot
save.image('myImage.Rimage')
```

<h2>Load</h2>

```r
# Load an object or severl objects (including the image)
load('path/to/the/file/myObjects')
```

<h2>Install packages</h2>

```r
install.packages(c('ggplot2', 'svmpath'， 'e1071'))

# Sometimes PeterMac blocks the access from CRAN,
# therefore install.packages() from CRAN will not work.
# In this case, you can download the zip file from CRAN,
# and install from local zip.
install.packages('path/to/the/zip/gglot2.zip', repos=NULL)
```
