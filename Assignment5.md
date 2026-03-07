**Assignment 5: SQl Basics**

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

I used the 2015_murder column from murder_2015_final.csv beause
