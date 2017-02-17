>#### Data Analysis: Steps
1. After downloading files, I opened the 2010 file and created a table.  Then I clicked the "Sort & Filter" button.  
2. In "School Type" column, I removed Foreign For-Profit, Private, and Public.
3. I didn't want to have to check every single zip code for the ending digit in the "Zip Code" column, so I googled how to select only a particular character in excel.  I found that using the LEFT and RIGHT function would let me select a particular character from any direction, so I created a new column just for the last digit of the zipcode and used =RIGHT(##, 1) in order to pick the last digit in each zipcode. From this column, I filtered out any row with the digit 3, 5, or 7.
4. At this point I repeated my process for the 2015 file and began answering the questions.

**Question 1** 
_Consider all of the schools that disbursed a total of more than $25,000,000 in loans during a single quarter. How many more schools met this criteria in 2015 than in 2010?_

#### 12 more schools met the criteria in 2015.

To find the total amounts disbursed for each school, I had to create a new column and write a formula to add up the values from the six columns labeled $ of disbursements.  The formula I wrote was =SUM(##, ##, ##, ##, ##, ##). To remove the schools that disbursed less than $25,000,000 in loans for the quarter, I went back to the column head and filtered only the amounts greater than or equal to that amount.  I noticed that the row numbers listed on the left were skipping numbers (and when I clicked "unhide row" it brought back an item I had previously filtered out), so I copied the table into a new worksheet to ensure I had the right total for the number of schools.  For the year 2010, I counted 225 schools and for the year 2015, I counted 237 schools. I felt this might be incorrect because I would have expected the number to have gone up more, and I was unsure why the 2015 report had fewer loan types than 2010.  It turns out that the report simply combines two types from before (DL SUBSIDIZED GRADUATE and UNDERGRADUATE are merged into one category), but even after completing this process a second time I still found a difference of only 12 schools.

**Question 2**
_For each state calculate the number of recipients for undergraduate student loans at non-public institutions in 2015. What was the largest difference between subsidized and unsubsidized loans in a single state?_

Since this question asks only about non-public institutions, I first filtered out all of the public schools.  Then, I copied the State, Recipient (Subsidized), and Receipient (Unsubsidized- Undergraduate) into a new worksheet so I had less to deal with.  I created a new table including only one instance of each state in a new table.  I used the 

**Question 3**
_Compare HBCUs established prior to the Reconstruction Era and those established during Reconstruction. Which group had the largest change in number of loan recipients between 2010 and 2015?_

Possible answers:

- Prior to the Reconstruction Era
- During the Reconstruction Era
- Both groups had the the same change
- It's not possible to determine this with the provided data
