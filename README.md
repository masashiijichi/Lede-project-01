# lede-project-01
This is project-01 homework for lede program
<br>
Link to the project-01 (https://masashiijichi.github.io/lede-project-01-website/doc/lede_project.index.html)

# Title
Reading Japanese baby’s name is getting harder
<br>
-Government decided to ask citizens to clarify how to read-


# Finding
Newborn Japanese baby name is getting more and more complexed.  The number of strokes are increasing and the variety of readings are also increasing.  

# Summary of data collection process
1. Extract popular baby names by year from this website (https://www.meijiyasuda.co.jp/enjoy/ranking/index.html#/year/2023n)


2. Use this API (https://kanjiapi.dev/) to get strokes and other information

# Overview of the data analysis process
1. Access meijiyasuda website from year 1912 to year 2023
2. Create a dataframe of top 10 popular baby names by year and by gender
3. Split each name by letter
4. Find strokes and other information for these letters by kanjiAPI
5. Create another dataframe of Chinese characters found in baby names
6. Merge these two dataframes
7. Count the strokes and the readings of each name

# A section about what new skills, approaches, etc you used, or where you grew the most during the project
1. Adding API info to HTML scraping was new approach
2. Using GIF in webpage was new skill (I used following websites)
   <br>
   https://kakijun.jp/
   <br>
   https://www.writehiragana.de/katakana.html
3. Using Ezgif to edit GIF was new skill
   <br>
   https://ezgif.com/
4. Creating a webpage was new skill
5. Creating a github page with detailed necessary info was new skill

# A section about things you tried to do or wanted to do but did not have the skills/time (but if you have more time you might do)
1. Adding scrolly function
2. Adding interactive functions to experience the increasing complexity of Japanese names
3. Analyzing data from different angle (is there a trend for the meaning of Chinese character used in Japanese names?)
4. Interviewing experts on this area and parents who have a child
   

# About this repository

### index HTML
[index HTML](doc/lede_project.index.html) - an index html
### jupyter notebook
[code 1](JPN_baby_name.ipynb) -  a Python file to scrape data from HTML website, to access API and to analyze dataset
### data 
[main data](data/jpnbabyname0704.xlsx) - an excel file with all the data
<br>
[stroke data](data/jpbaby_gender_stroke.xlsx) - an excel file for stroke data fit for flourish format
<br>
[reading data](data/jpbaby_gender_reading.xlsx) - an excel file for reading data fit for flourish format
<br>
*all the data are stored in excel format in case encoding for various Japanese/Chinese letters don't work in csv format
