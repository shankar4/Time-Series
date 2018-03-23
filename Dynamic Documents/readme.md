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
