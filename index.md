## Assingment 07: Functions

### Introduction
This week’s lesson was primarily focused on functions.  A function is a named piece of SQL code used to perform a task.  There are many built in functions, and users can also create their own functions (User Defined Functions, UDF).

### Explain when you would use a SQL UDF
SQL UDFs are used to store a piece of code used to perform an action and have it easily recalled later when necessary.  Creating a function and calling it later is a way to keep code organized as well.  When the operation is required multiple times, a user define function is an efficient method to accomplish this. Figure 1 below shows an example of this assignments UDF.


![Figure 1 UDF](https://user-images.githubusercontent.com/74632205/101220768-4227f600-3654-11eb-9994-b411d33cd9a2.PNG)

***Figure 1: Example of UDF, user selects which KPI value to include in the returned table***

### Explain the differences between a Scalar, Inline, and Multi-Statement Functions

Scalar functions return only a single value.  The data type of the single value in the RETURNS clause of the function must be identified.  In Figure 1, this is done in line 326 (@KPIvalue int).  Inline functions only need RETURNS TABLE specified and the table’s definition will be based on the functions SELECT statement.  A BEGIN/END syntax is not needed for an inline function.  Multi-Statement functions have a RETURNS syntax that specifies the structure of the return table.  A BEGIN/END syntax is required for a multi-statement function.
