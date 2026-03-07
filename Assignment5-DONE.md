**Assignment 5: SQl Basics - DONE**

*Final SQL Query*

SELECT
    murder_2015_final.city,
    murder_2015_final.state,
    murder_2015_final."2014_murders",
    murder_2015_final."2015_murders",
    murder_2016_prelim."2016_murders"
FROM murder_2015_final
JOIN murder_2016_prelim
ON murder_2015_final.city = murder_2016_prelim.city
AND murder_2015_final.state = murder_2016_prelim.state
ORDER BY murder_2016_prelim."2016_murders" DESC;

<img width="672" height="426" alt="Screenshot 2026-03-07 at 1 16 35 PM" src="https://github.com/user-attachments/assets/e1d9a62b-8f95-4643-9f2b-fd8370d319c5" />

I used the 2015_murder column from murder_2015_final.csv because I was able to cooroborate that data with reputable sources. An article from the [New York Times](https://www.nytimes.com/2016/09/27/us/murder-crime-fbi.html) referencing a report released by the FBI states that New York saw 352 murders in 2015, Los Angeles saw 282, and Milwaukee saw 145. All three stats matched the data found in murder_2015_final.  
