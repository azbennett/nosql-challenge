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

I used the regex to search for London in the LocalAuthorityName to solve it eventually.

* https://pynative.com/python-regex-compile/
* https://www.w3schools.com/python/python_regex.asp
* https://docs.python.org/3/library/re.html

