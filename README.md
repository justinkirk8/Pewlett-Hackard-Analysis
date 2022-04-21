# Pewlett-Hackard-Analysis
## Overview of Analysis:
Client wanted their current database being kept in excel to be updated to a SQL database in PostgreSQL. Client is also concerned about number of upcoming retiring employees in the company. Client is requesting the following tables.
- A count of retiring employees based on current position title.
- A table of current employees who could potentially take part in a mentorship program base on what year they were born which includes: employee number, name, date of birth, hire date, and current position title.

## Resources
- Software: pgAdmin4, PostgreSQL 14

## Results
- The number of managers retiring small which will indicate the company won’t be losing much of its leadership structure during the transition.
- Conversely, the two largest retiring categories are Senior Engineer and Senior Staff. This indicates that the company will be losing a significant amount of experience and skills. 
- Further, another category which is concerning is the Technique Leader which has 3603 retirees. This indicates employees who possess a large amount of technical knowledge. This, and the above point, strongly supports the need for the mentioned mentorship program. 


<p align="center">
  <img src="https://github.com/justinkirk8/Pewlett-Hackard-Analysis/blob/main/Images/retirement_title_count.png" width="300" />
</p>

- Based on the provided search criteria, there are 1549 employees eligible for the mentorship program.

- Further filtering of the table shows that there are 77 Technique Leaders that are eligible for the mentorship program which should possess more knowledge and provide a better outcome in a mentorship role.

## Summary
The summary addresses the two questions and contains two additional queries or tables that may provide more insight.
The large group of upcoming retirees consists of several different titles; however, the largest groups are Senior Engineer and Senior Staff which represent a significant amount of experience and skills. Further, many Technique Leaders are retiring who represent a large amount of technical knowledge. This largely supports the needs for the mentorship program. The provided parameters for the mentorship program table result in 1549 candidates, however, further examination of the table shows that it includes titles such as assistant engineer which are less likely to have the technical knowledge to succeed in a mentorship position. Two adjustments to the mentorship program search parameters and the following were the results:
- The request for mentorship eligibility was adjusted to remove the birthday parameter and limit the job title to Technique Leader.  This provided a list of 12 thousand employees who could be good candidates for the mentorship program in order to pass on technical knowledge. This table can be found in the mentorship_eligibility_alt1.csv.
- The request for mentorship eligibility was adjusted to cover a 10-year period of birthdays (from 1956 to 1965) and the job title was limited to Senior Engineer and Senior Staff. This provided a list of 117 thousand employees who are within 10 years of the provided retirement year who could be good candidates for the mentorship program in order to pass on their experience and skills.
