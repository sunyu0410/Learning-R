<h1>Some routines  in R</h1>

```r
# To quit R, use q()
# You will be asked whether to save the image (whole environment).
# It is better to explicitly save what you want (see below).
q()

# Save, save, save
# Command history (all commands typed)
savehistory('myhistory.txt')
# An object of interest
save(list_of_object, file='myobject.Robject')
# All objects (the whole environment), 
# also called an image or a snapshot
save.image('myImage.Rimage')

# Load an object or severl objects (including the image)
load('path/to/the/file/myObjects')

# Install packages
install.packages('ggplot2')

# Sometimes PeterMac blocks the access from CRAN,
# therefore install.packages() from CRAN will not work.
# In this case, you can download the zip file from CRAN,
# and install from local zip.
install.packages('path/to/the/zip/gglot2.zip', repos=NULL)
