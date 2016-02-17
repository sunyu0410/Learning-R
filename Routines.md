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
# Install a list of packages
install.packages(c('ggplot2', 'svmpath'， 'e1071'))

# Sometimes PeterMac blocks the access from CRAN,
# therefore install.packages() from CRAN will not work.
# In this case, you can download the zip file from CRAN,
# and install from local zip.
# see http://stackoverflow.com/questions/7075709/install-binary-zipped-r-package-via-command-line
install.packages('path/to/the/zip/gglot2.zip', repos=NULL)
```

<h2>Run a script</h2>

```bat
Rscript myscript.r
```

<h2>Run R non-interactively</h2>
```bat
:: Sometimes you just want to execute a script 
:: and store the result in a text file.
R CMD BATCH input.r output.txt

:: To run it in background, add & at the end.
:: This is suitable for cloud computing.
R CMD BATCH input.r output.txt &

:: To see the process
top
```
