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
**#Medium 2**
This code is an implementation of the Boyer-Moore Majority Vote algorithm to find the majority elements in an array. The algorithm is designed to find elements that appear more than n/3 times in an array, where n is the length of the array.
Initialize two candidate elements (candidate1 and candidate2) and their corresponding counts (count1 and count2) to None and 0.
Iterate through the array (nums) and update counts for the candidates.
If the current number matches either candidate, increment the corresponding count.
If the counts are zero, update the candidate and set the count to 1.
If counts are not zero, decrement both counts.
Reset counts for the second phase.
Iterate through the array again and count the occurrences of the potential candidates.
Check if the counts of candidates meet the criteria for majority elements (more than n/3 occurrences).
If so, append the candidates to the result list.
Return the list of majority elements.
**Hard 2**
 The algorithm uses the KMP (Knuth-Morris-Pratt) pattern matching algorithm to find the longest palindrome that is also a prefix of the given string.
 Create a modified string by concatenating the original string (s) with its reverse and adding a special character ("#") in the middle.
Initialize a KMP table (kmp_table) with zeros.
Initialize an index j to track the current position in the pattern.
Use the KMP algorithm to build the KMP table.
Iterate through the modified string, updating the table based on pattern matches.
Get the length of the matching prefix (the longest palindrome that is also a prefix) from the last value of the KMP table.
Extract the suffix of the original string (s) starting from the length of the matching prefix.
Reverse the extracted suffix and concatenate it with the original string to form the shortest palindrome.
Return the shortest palindrome.
