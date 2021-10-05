# Question and difficult point

##  579. https://leetcode.com/problems/find-cumulative-salary-of-an-employee/
### 1) cumulative salary: the time column should be both threshold and variable
#### hint: self join with a.time to be index and b.time to vary
#### Example: subquery should be used to define the new column (select salary from employee where month=b.month-1 and id=b.id )
### 2) in case syntax, else 0 may still output NULL, then you need to use ifnull to convert null into 0
### 3) calculate the column summation within each row: need to use column A + column B + column C instead of sum(A+B+C)
## 601. https://leetcode.com/problems/human-traffic-of-stadium/
### 1) consecutive days with people more than 99
#### hint: row_number in general - row_number under special case
## [2]615. https://leetcode.com/problems/average-salary-departments-vs-company/
### 1) when using window function instead of group by, you should use distinct to manually filter unique row records.
## 618. https://leetcode.com/problems/students-report-by-geography/
### 1) pivot the table only needs to use the row_number as clue to show all the first value in first row and etc
