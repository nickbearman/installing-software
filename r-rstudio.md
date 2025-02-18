## Installing R & RStudio

We will be setting up R & RStudio. Follow the instructions below, depending on your operating system, and the follow the library installation section.

## Windows 

- Open a web browser and go to [https://cran.r-project.org/](https://cran.r-project.org/){:target="_newpage"}. 
- Click **Download R for Windows**. 
- Choose the link **install R for the first time**. 
- Download the latest version (4.4.2 at time of writing) **Download R-4.4.2 for Windows**. 
- Run through the program installation process.  
- Once R is installed, we can install RStudio. 
- Go to [https://posit.co/download/rstudio-desktop/#download](https://posit.co/download/rstudio-desktop/#download){:target="_newpage"}. 
- Download the latest version (2024.12.1+563 at the time of writing). 
- Under **2: Install RStudio** click **DOWNLOAD RSTUDIO DESKTOP FOR WINDOWS**
- Run through the program installation process.  

## Mac / OS X

- Open a web browser and go to [https://cran.r-project.org/](https://cran.r-project.org/){:target="_newpage"}. 
- Click **Download R for macOS**. 
- Download the latest version (4.4.2 at time of writing) **R-4.4.2-arm64.pkg**. 
- Run through the program installation process.  
- Once R is installed, we can install RStudio. 
- Go to [https://posit.co/download/rstudio-desktop/#download](https://posit.co/download/rstudio-desktop/#download){:target="_newpage"}. 
- Click **DOWNLOAD RSTUDIO DESKTOP FOR macOS**
- Download the latest version (2024.12.1+563 at the time of writing). 
- Run through the program installation process. 

<!-- add later
##Linux/Ubuntu

- Open a web browser and go to https://cran.r-project.org/.   
- Click **Download R for Linux**.  
- Go into the relevant Linux distribution
- Follow the instructions for the appropriate Linux distribution.  
<!-- add more to this section -->

## Libraries

R uses libraries to add features and different tools, such as GIS and spatial analysis. We need to install some libraries we will be using. 

- Open **RStudio**. 
- In the **Console** type in `install.packages("sf")`. 
- Then load the library by running `library(sf)`. 
- Check the output you get - red text does not always mean an error! 
- Repeat the process for the `tmap` package (`install.packages("tmap")` and then `library(tmap)`) and any other packages you need. 

*If you already have `tmap` installed, please upgrade it to the latest version. We will be using `tmap` v4 in the course. If you are not sure which version of `tmap` you are using, you can check by loading `tmap` and then running `packageVersion("tmap")`.*

If you get stuck, check out [troubleshooting](r-rstudio-library-troubleshooting.html) for some things to try. 

## Posit Cloud

If you can't get R & RStudio installed on your computer, there is another option. You can use Posit Cloud, which runs RStudio in a web browser. You can get a free account which will be enough for a short course. 

- Go to [posit.cloud](https://posit.cloud/){:target="_newpage"}.
- Choose **Sign Up** 
- Select **Learn more** under the **Cloud free** plan 
- Choose **Sign Up** and fill out the form. 
- To get started, choose **New Project** and **New RStudio Project**. *It will take a few seconds to load*. 


## Troubleshooting

If you get stuck, check out [troubleshooting](r-rstudio-library-troubleshooting.html) for some things to try. 

You are good to go!

*This work is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit [http://creativecommons.org/licenses/by-sa/4.0/deed.en](http://creativecommons.org/licenses/by-sa/4.0/deed.en). The latest version of this is available from [https://nickbearman.github.io/installing-software/r-rstudio](https://nickbearman.github.io/installing-software/r-rstudio).*
