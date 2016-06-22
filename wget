# Wget
Hey, Wget is pretty cool. Why didn't I figure this out before?

I used this script to download CMIP5 climate data sets for use in my research. This script is recursive (-r), grabs data from other hosts (-H)
ignores the parent directory of the target URL (-np), ignores pesky robots, makes sure to includes zip files, and some other things that I can't remember now.
~~~~
wget -r -H -np -e robots=off -A .zip -p -E --cut-dirs=1 http://worldclim.org/cmip5_30s
~~~~
