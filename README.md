# nosql-challenge
# Steve Bennett 

Files used:
Resources/establishments.json

Import line: mongoimport --type json -d uk_food -c establishments --drop --jsonArray Resources/establishments.json

NoSQL_setup_starter.ipynb
NoSQL_analysis_starter.ipynb

Items of note from the analysis_starter:

Question 2. Which establishments in London have a `RatingValue` greater than or equal to 4?

I Noticed when looking through the data that we had a very inconsistent data entry of where London is placed. For some establishments it was on line2, 3 or 4.  

One would have suspected that "LocalAuthorityName" was the field I wanted here, but ZERO results contain "London" in the original data source file.

Not sure if the question is outdated for a previous dataset, or purposely designed to trick us.

I also noticed that sometimes there was a "London Road" and just using a normal regex search resulted in that data being included.  So I used import re to help ensure ONLY exactly London was within my results.

* https://pynative.com/python-regex-compile/
* https://www.w3schools.com/python/python_regex.asp
* https://docs.python.org/3/library/re.html

