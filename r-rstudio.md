---
title: "Installing R & Rstudio"
author: "Nick Bearman"
output:
  pdf_document: default
  html_document:
    df_print: paged
---

We will be setting up R & RStudio. Follow the instructions below, depending on your operating system, and the follow the libray installation section.

## Windows 

- Open a web browser and go to https://cran.r-project.org/. 
- Click **Download R for Windows**. 
- Choose the link **install R for the first time**. 
- Download the latest version (3.5.3 at time of writing) **Download R 3.5.3 for Windows**. 
- Run through the program installation process.  
- Once R is installed, we can install RStudio. 
- Go to https://www.rstudio.com/products/rstudio/download/#download. 
- Download the latest version (1.2.1335 at the time of writing) **RStudio 1.2.1335 - Windows 7+**. 
- Run through the program installation process.  

## OSX

- Open a web browser and go to https://cran.r-project.org/. 
- Click **Download R for (Mac) OS X**. 
- Download the latest version (3.5.3 at time of writing) **R-3.5.3.pkg**. 
- Run through the program installation process.  
- Once R is installed, we can install RStudio. 
- Go to https://www.rstudio.com/products/rstudio/download/#download. 
- Download the latest version (1.2.1335 at the time of writing) **RStudio 1.2.1335 - Mac OS X 10.12+ (64-bit)**. 
- Run through the program installation process. 

<!-- add later
##Linux/Ubuntu

- Open a web browser and go to https://cran.r-project.org/.   
- Click **Download R for Linux**.  
- Go into the relevant Linux distribution
- Follow the instructions for the appropiate Linux distribution.  
<!-- add more to this section -->

## Libaries

R uses libaries to add features and different tools, such as GIS and spatial analysis. We need to install some libaries we will be using. 

- Open **RStudio**. 
- In the **Console** type in `install.packages("sf")`. 
- Check the output you get - red text does not always mean an error! 
- Repeat the process for the `tmap` package (`install.packages("tmap")`). 


You are good to go!

*This work is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/deed.en. The latest version of this is available from https://github.com/nickbearman/installing-software. This version was created on 12/04/2019.*
