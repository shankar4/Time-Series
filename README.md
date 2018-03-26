### Time-Series
Practical R programs for time series analysis
The early part is based on "Practical Time Series" by Gareth and Janacek, 2001. I visited Dr. Janacek's website and publicly available links for downloads to reconstruct the material/software covered/used in their book (the original links are not functional). There are other R packages that can be used in place of these earlier packages. This will be done as and when necessary (and documented here).

I will also use 'Dynamic Documents with R and knitr' 2nd edition, by Yihui Xie, 2015, to build dynamic reports (combines narrative and embedded R code that is executed to generate appropriate output). 

At present, all the info downloaded from the web, as pertinent to Dr. Janacek's books and class material, is at my Googledoc site. Over a period of time, some of the data will get integrated into examples and compiled with knitr, and made available here in that format (as .Rmd and .html files).

All the data is in TimeSeries.zip. The updated .Rmd files use the unzipped directory as the working directory for compiling the code with knitr, so the code is totally reproducible. This also means that the working directory is set to the source document before knitr is called. It was difficult to include all the source code up front. So, there is a lot of data duplication, as more source code is added. Also, I have used newer R packages as appropriate.
1. V1 has tsplot and splot on wheat data and source code (.rmd and .html) that uses Janacek's code for these two functions.
2. V2 has V1 plus source code for moving average with sma() function of 'smooth' package. 


'smooth' is a new smoothing package. References: https://github.com/config-i1/smooth/blob/master/inst/doc/smooth-Documentation.pdf and https://cran.r-project.org/web/packages/smooth/vignettes/smooth.html . 
