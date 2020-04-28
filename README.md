# cs424-project3
The following was coded on a Windows PC using languages R and Python. IDE's used for R are RStudio, and for Python is PyCharm.

Languages and IDE's can be downloaded here:
https://www.python.org/downloads/
https://cran.r-project.org/mirrors.html

https://www.jetbrains.com/pycharm/download/#section=windows
https://rstudio.com/products/rstudio/download/

Files are too big to upload on here so download the zip file from:
https://drive.google.com/file/d/1AnChFQD631u1O8tx5RMf-SCcZxp8w6w_/view?usp=sharing

Download data
ftp://ftp.fu-berlin.de/pub/misc/movies/database/frozendata/

The specific files downloaded for this project is:
release-dates.list
running-times.list
certificates.list
genres.list
keywords.list
movies.list
ratings.list

Unzipping Data
Since the data comes in a GZIP format, I was able to unzip it by the following manner:
1.       I downloaded the program WinSCP
a.       found at https://winscp.net/eng/index.php
2.       I connected to an external server at my school which hosts file extraction software
3.       I connected to the system1 server at UIC through SSH through Windows PowerShell
4.       In systems1 I unzipped the .gz extension files by using command
a.       gunzip <filename.gz>
5.       I then transferred back the unzipped files to my PC through WinSCP
I did some research and there exists an open source software called 7-Zip found at: https://www.7-zip.org/ that could be used to extract the zipped files needed for this project.

Make sure when you unzip the data, store it in "python scripts" folder of "IMDB_atimoc2_proj3" project. 

Run python preprocessing scripts with command:
python "names of script" 
for example) python keywords_pre.py

After running all python scripts rename folder "python scripts" to "data".
Then you can run R scripts to create the associated RData structure files for the application.


If you are feeling lazy all the processing has been done for you and you can open app.R in RStudio, and run the application.
Make sure that you have a shinyapp account to do so. Otherwise skip all this and just take a look at the visualization at my shinyapp site: https://atimochina.shinyapps.io/IMDB_atimoc2_proj3/


