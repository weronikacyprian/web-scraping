# Web scraping from the repository of Polish translations of Shakespeare
This project aims to create a table with clear information from the repository of Polish translations of Shakespeare (https://polskiszekspir.uw.edu.pl/).

I wanted to implement a way to crawl information such as the title of publication, author (as in translator), year and place of publication, and the name of the publisher; all from the target website. Then, I created and displayed a table that contained these unique records. The table consists of five columns: the row number in the table, publication title, author, year, place of publication and publisher. 

This code was implemented taking into consideration handling possible errors, validation and the best visualisation of data from web scraping, also being user-friendly.

I tried to break down the code into specific functions such as "extract_publications", or "display_table_enhanced", so it is much easier to follow and possibly update. Each of the function covers different part of the process of this task, keeping in mind clean code organisation.

In "extract_publications" function I made sure to filter out the unwanted words that were appearing in the title entries, as well as non-author text. It was completed by implementing efficient text processing expressions. I decided to use r library for this purpose.

At the end, in "display_table_enhanced" I am using Pandas library to create a nicely looking styled DataFrame, which displays publications with their yea, names of authors, place of publication and titles.


