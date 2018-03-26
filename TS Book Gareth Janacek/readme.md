I have rearranged and limited the material covered to topics of immediate interest to me:
1. The R language for Time series
2. Time Domain - Moving Averages
3. Frequency Domain - Frequency and Power Spectrum

At present, all the info downloaded from the web, as pertinent to Dr. Janacek's books and class material, is at my Googledoc site. Over a period of time, some of the data will get integrated into examples and compiled with knitr, and made available here in that format (as .Rmd and .html files).  

All the data is in  TimeSeries.zip. The updated .Rmd files use the unzipped directory as the working directory for compiling the code with knitr, so the code is totally reproducible. This also means that the working directory is set to the source document before knitr is called. It was difficult to include all the source code up front. So, there is a lot of data duplication, as more source code is added. Also, I have used newer R packages as appropriate. 

1. V1 has tsplot and splot on wheat data and source code (.rmd and .html) that uses Janacek's code for these two functions. 
2. V2 has V1 plus source code for ....
