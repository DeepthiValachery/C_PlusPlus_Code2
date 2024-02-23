# C_PlusPlus_Code2
My Second C++ Code

The Central Statistical Office (CSO) of Trinidad and Tobago has produced summary data on the results obtained by primary school students writing the Secondary Entrance Examination (SEA) from 2010 to 2018. The data is shown in the following table1.

[TABLE]

Table 1 shows three categories of data for each year:

• Category 1: Number of students getting ≤ 30%

• Category 3: Number of students getting ≥ 50%

• Category 4: Number of students getting ≥ 90%

The table does not give data for Category 2, the number of students getting < 50%. However, this can be calculated from the other data.

This assignment requires you to perform some simple analyses on the data for a given period, which is specified by the user at the keyboard. You are also required to produce a graph.

PROGRAM REQUIREMENTS

Write a program which:

1. FIRST, prompts the user to enter the starting year for the analysis and the ending year for the analysis, subject to the following:

• The starting year could be the same as the ending year (so only one year is analysed).

• The starting year and the ending year must be between 2010 and 2018 (inclusive). Otherwise, your program should display an error message and terminate.

• If the starting year is greater than the ending year, the values are swapped so that the starting year becomes less than the ending year.

2. THEN, for EACH year in the analysis period, the following actions should be performed:

• The user is requested to enter the number of students who wrote the exam, and the number of students in Category 1, Category 3, and Category 4.

• The number of students in Category 2 should be calculated based on the number of students who wrote the exam and the number of students in Category 3.

• The percentage of students in each category should be calculated and displayed.

• The highest number of students getting ≥ 90 in all the years being analysed should be found.

• The lowest number of students getting < 50 in all the years being analysed should be found.

3. AFTER the data for all the years to be analysed has been entered by the user, the program should display the following:

• The average number of students in Category 1, Category 2, Category 3, and Category 4. The average must be a whole number (use the floor function to truncate the fractional part).

• The percentage of students in each category (based on the average).

• The highest number of students getting ≥ 90 and the year it occurred.

• The lowest number of students getting < 50 and the year it occurred.

4. NEXT, a graph must be drawn showing the average number of students in each category. The graph consists of a set of asterisks on a line for each category. One asterisk (‘*’) is displayed for every 500 students in the average for each category.
