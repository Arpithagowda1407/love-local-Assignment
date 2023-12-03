# love-local-Assignment
**#Easy 3**
The function starts by checking if numRows is 0. If it is, an empty list is returned since Pascal's Triangle with 0 rows is an empty triangle.
The variable triangle is initialized with the first row, which is [1]. This represents the first row of Pascal's Triangle.
The function then enters a loop from 1 to numRows - 1. This loop generates each subsequent row of Pascal's Triangle.
Inside the outer loop, a new list row is created for each row, starting with the value 1.
An inner loop runs from 1 to i - 1 to fill in the middle elements of the row. For each middle element, the value is the sum of the two elements directly above it in the previous row.
After the inner loop, the last element 1 is appended to the row.
The completed row is then appended to the triangle, representing a new row in Pascal's Triangle.
Steps 4-7 are repeated for each row until the desired number of rows (numRows) is reached.
The final triangle is returned, representing Pascal's Triangle with the specified number of rows.
