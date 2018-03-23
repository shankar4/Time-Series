This is based on "Dynamic Documents with R and knitr', 2nd edition, by Yihui Xie, 2015.
The original idea for this, literate programming,  came from Donald Knuth: "Instead of imagining that our main task is to instruct a computer what to do, let us concentrate rather on explaining to humans what we want the computer to do." Reproducible Research (RR), as envisioned by Jon Claerbout,  is facilitated (at least partially) by dynamic documents. The knitr package, developed by Yihui Xie, supports this. Xie lists these practices to make our code portable so we come close to RR:
1. Manage all source files under the same directory and use relative paths. Make an archive (e.g., zip) of the whole directory for distribution
2. Set to this directory of source files before knitr is called. 
3. Compile the documents in a clear R session
4. Avoid commands that require human interaction
5. Avoid environment variables for data analysis
6. Attach *sessionInfo()* and instructions on how to compile this document. 

RR has some barriers:
1. Difficult to archive large amounts of data and distribute with the code. Provide Urls
2. Confidentiality of data
3. Software may run differently on different operating systems/versions
4. Potential competitors can get all the code for free

Set up: In Rstudio, type: 
>install.packages("knitr", dependencies=TRUE)

'showtext' had non-zero exit. I tried to install 'showtext' package again. This failed with a suggestion to install libfreetype6.dev, in cmd shell:
>sudo apt-get install libfreetype6-dev

After this, I reinstalled 'showtext' and then knitr (as given above). It was successful. 

I also installed 'shiny' package to help with web pages (html). 

'A Minimal Example' is covered in his chapter 3. In RStudio, use File --> New File --> R Markdown. Once the document is ready, click the **knit** button. A document will be generated that includes both narrative and output of embedded R code. It is saved as 'A Minimal Example.Rmd'. (R markdown url: rmarkdown.rstudio.com). After clicking the kint button, this file is generated: 'A_Minimal_Example.html.' I clicked the 'Publish' button at the right hand side top. Rstudio suggested that I install PKI, rsconnect. I installed them. These will help me publish at RPubs and RStudio Connect. Will save it for some really good examples from me! For now, launch the .html file attached here in a web browser to see the result. This is not easy from Github, unless you download all of the files as a zip file. Here is the way to do it directly from Github. First launch this link in a new browser window: http://htmlpreview.github.io/ -- Right click and copy the html page link, and paste it in the box in that window. Hit the >> icon, and your html page will render properly. 

The knitr package reference site is [here](https://yihui.name/knitr/). 



