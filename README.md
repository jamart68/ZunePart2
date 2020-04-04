# ZunePart2

So what’s the purpose of the while loop? To put it simply, it’s designed to get the number of years from the number of days since 1980 as well as a remainder of days out of the current year. Keep in mind that you’re never supposed to retry the loop without committing some sort of action which will ultimately exit the loop:

1.	year is set to ORIGINYEAR. Since ORIGINYEAR is 1980, any addition to year is added on top of 1980. This is fine because the hardware is passing the number of days since January 1, 1980. 
2.	Is the number of days greater than 365? If so, proceed. Otherwise, skip to number 6. 
3.	Is the current year a leap year? If so, proceed. Otherwise, subtract 365 from the number of days, add 1 to the number of years, and skip to number 5. 
4.	Is the number of days greater than 366? If so, subtract 366 from the number of days, add 1 to the number of years, and proceed. 
5.	retry number 2. 
6.	This is the loop exit point – success if you get here
