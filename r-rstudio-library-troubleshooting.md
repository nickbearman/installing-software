## Installing R & RStudio Libraries - Troubleshooting

Installing Libraries in R can be problematic sometimes. Here are a few hints and tips that might be useful for you.

## Install sf

R uses libraries to add features and different tools, such as GIS and spatial analysis. We need to install some libraries we will be using. Follow these instructions to install the `sf` library. *Note the terms library and package are interchangeable.*

- Open **RStudio**.
- In the **Console** type in `install.packages("sf")` and press enter.

This is (approximately) the output you should get (click the link for the full image):

[![](images/r-install-packages-sf-success-cut.png)](images/r-install-packages-sf-success-full.png)

- Then load the library by running `library(sf)`.

- Check the output you get - red text does not always mean an error!

## Install tmap

- Repeat the process for the `tmap` package.
- In the **Console** type in `install.packages("tmap")`.

This is (approximately) the output you should get (*I've not included the full version because it is so long!*):

![](images/r-install-packages-tmap-success-cut.png)

- The load the library by running `library(tmap)`. 

- The `tmap` library may give you this message:

![Breaking News: tmap 3.x is retiring. Please test v4, e.g. with
remotes::install_github('r-tmap/tmap')](images/tmap-v4-testing.png)

This is saying that there is a new version of the `tmap` library - version 4. It is not out yet and RStudio will have installed version 3.3-4 for you. We will stick with using version 3 in this course, and I will talk more about this in the presentation. 

## Problems

If you don't get this output, there may have been a problem. Best move is to try loading the libraries again.

- In the **Console** type in `library(sf)`.
- and then type in `library(tmap)`.

You should get something like this:

![](images/r-load-library-success-sf-tmap.png)

If you don't, then there are a few steps you can try:

- R might say a dependent library is unavailable. 
	- Check what the red text says. If it says (for example) `There has been an error installing the Rcpp library`, try installing that library:
	- `install.packages("Rcpp")`
	- Then try loading it: `library(Rcpp)`
	- If that works, try installing either `sf` or `tmap` again.
- R might ask if you want to compile the package from source:
	![](images/r-binary-version.png)
	- Usually the best choice here is to say no, which means R will use a very slightly older version of the library, but it should be fine for our work. 
	- *If you say yes, R will ask you to install RTools, which will probably work, but adds to the length of the setup time!*
	
- R might give you instructions to install another piece of software - try this if you can.
 
- If none of those work, you can try uninstalling and reinstalling the library
	- Remove using `remove.packages("classInt")` (*e.g. for the `classInt` package*) or
	- Open the **Packages** tab (on the right) and click the `X` by whichever package you want to remove:
	
	![](images/r-remove-packages.png)
	
- If that doesn't work, do reach out to me before the course and ask for help.

- An alternative is to use [RStudio.cloud / Posit.cloud](r-rstudio.html#posit-cloud). 

*This work is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit [http://creativecommons.org/licenses/by-sa/4.0/deed.en](http://creativecommons.org/licenses/by-sa/4.0/deed.en). The latest version of this is available from [https://nickbearman.github.io/installing-software/r-rstudio](https://nickbearman.github.io/installing-software/r-rstudio).*
