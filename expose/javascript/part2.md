1) Line 12 will print "3". This is because that is the value of i when the loop ends and line 12 logs the value of i to the console right after the loop ends so thats why it prints "3".

2) Line 13 will print "150". This is because on the last iteration of the loop, discountedPrice is set to prices[2] * (1 - 0.5), which evaluates to 150. That is the value of the variable discountedPrice on the last iteration of the loop, so thats what the value of the var will be after the loop is done. Since 150 is what is stored and line 13 logs to the console right after the loop ends, line 13 prints "150".

3) Line 14 will print "150". This is because on the last iteration of the loop, finalPrice is set to Math.round(150 * 100) / 100, which evaluates to 150. That is the value of the variable finalPrice on the last iteration of the loop, so thats what the value of the var will be after the loop is done. Since 150 is what is stored and line 14 logs to the console right after the loop ends, line 14 prints "150".

4) The function will return the array [ 50, 100, 150 ]. This is because those are the discounted values of the three input prices 100, 200, 300, respectively. We defined "discounted" as an array at the beginning and push each price after it is calculated so thats why it is an array with the discounted prices in the order of the original input values.

5) Line 12 returns an error. Since we used the keyword let to declare "i", the scope is limited to the for loop block which is where it was declared. Since line 12 is outside of that block, when it tries to log i to the console i can not be reached so an error is thrown.

6) Line 13 returns an error. Since we used the keyword let to declare "discountedPrice", the scope is limited to the for loop block which is where it was declared. Since line 13 is outside of that block, when it tries to log discountedPrice to the console, discountedPrice can not be reached so an error is thrown.

7) Line 14 will print "150".  This is because on the last iteration of the loop, finalPrice is set to Math.round(150 * 100) / 100, which evaluates to 150. That is the value of the variable finalPrice on the last iteration of the loop, so thats what the value of the var will be after the loop is done. Since 150 is what is stored and line 14 logs to the console right after the loop ends, line 14 prints "150". Even though finalPrice was declared with let, since it was declared in the outer most part of the function the scope would be the block of the whole function, meaning line 14 is in scope and can access finalPrice.

8) The function will return the array [ 50, 100, 150 ]. This is because those are the discounted values of the three input prices 100, 200, 300, respectively. We defined "discounted" as an array at the beginning and push each price after it is calculated so thats why it is an array with the discounted prices in the order of the original input values. Since the return statement is in the same block as the variable discounted, it is able to access the array and doesn't throw any error.

9) Line 11 returns an error. Since we used the keyword let to declare "i", the scope is limited to the for loop block which is where it was declared. Since line 11 is outside of that block, when it tries to log i to the console i can not be reached so an error is thrown.

10) Line 12 prints "3" this is because the variable "length" stores the length of the input array "prices", and since there are 3 values in the input array "length" will be set to 3. 

11) The function will return the array [ 50, 100, 150 ]. This is because those are the discounted values of the three input prices 100, 200, 300, respectively. We defined "discounted" as an array at the beginning and push each price after it is calculated so thats why it is an array with the discounted prices in the order of the original input values.

12a) student.name
12b) student["Grad Year"]
12c) student.greeting()
12d) student["Favorite Teacher"].name
12e) student.courseLoad[0]

13a) The output for this arithmetic would be 32. When one of the operands is a string (in this case its '3'), the + operator is used for concatenation. Thats why the 2 is concatenated to the end of the '3', providing an output of 32.
13b) The output of this arithmetic is 1. Even though '3' is a string, it is converted to a number since the - operator can not be used for concatenation. After '3' is converted to a number 2 is subtracted from it giving an output of 1.
13c) The output of this arithmetic is 3. When using the + operator null is converted to the number 0. So the expression becomes 3 + 0 which just evaluates to 3.
13d) The output of this arithmetic is 3null. When one of the operands is a string the + operator is used for concatenation. null is treated as a string in this instance so it is just concatenated to the '3', producing an output of 3null.
13e) The output of this arithmetic is 4. When using the + operator true is converted to the number 1. So the expression becomes 1 + 3 which just evaluates to 4.
13f) The output of this arithmetic is 0. When using the + operator false is converted to the number 0 and null is also converted to the number 0. So this expression becomes 0 + 0 which just evaluates to 0.
13g)The output of this arithmetic is 3undefined. When one of the operands is a string, the + operator is used for concatenation. undefined is converted to a string which is concatenated to the '3' so the final output is 3undefined.
13h) The output of this arithemetic is NaN. When the - operator is used javascript tries to convert both values to numbers so it can perform subtraction. However undefined cannot be converted to a number so the output is NaN.

14a) The output of this comparison is true. When using the > operator both operands are converted into numbers. The '2' would be converted to a number so the expression would become 2 > 1, which evaluates to true since 2 is greater than 1.
14b) The output of this comparison is false. When using the < operator both operands are treated as strings and are compared character by character from left to right. Since the first character on the left is '2' and the first character on the right side is '1', it will return false since '2' comes after '1'.
14c) The output of this comparison is true. The == operator performs type conversion if the operands are of different types. The '2' would be converted to the number 2, so the expression would check if 2 is equal to 2, which returns true.
14d) The output of this comparison is false. The === operator checks type and value, and since '2' is a string but 2 is a number, the operator returns false as they are of different types.
14e) The output of this comparison is false. The == operator performs type conversion if the operands are of different types. True is converted to the number 1, so the operator checks if 1 is equal to 2. Since they are not equal it returns false.
14f) The output of this comparison is true. Any value other than 0 is considered as true by javascript. So when it is converted to a boolean, 2 becomes true. Now that they are both of the same type and of same value, the === operator would return true.

15) The difference between == and === operators is how they act when the two operands of different types. When they operands are the same type then both operators have the same behavior. When the operands have different types, the == operator will convert them to the same type and then compare them, so the type doesnt matter and only the actual value matters. On the other hand, the === operator performs the comparison without converting the type, so if the two operands are of different types then it will return false even though they are the same value. For example, '2' == 2 will return true since the '2' would be converted to a number, but '2' === 2 will return false as one operand is a string and the other is a number.

17) The function call will return the array [2, 4, 62]. First the code passes the array [1,2,31] to the modifyArray function. the modifyArray function loops through the input array and calls the doSomething function on each element of the input array. The results are added to the array newArr which is returned at the end. So the code basically loops through the input array and calls the input function on each element of the array.

19) The output is:
1
4
3
2
