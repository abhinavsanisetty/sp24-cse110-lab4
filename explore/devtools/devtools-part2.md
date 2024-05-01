1) The bug was that getElementById().value return string values even if they represent numbers. This means that instead of adding numbers, it is concatenating strings of the two numbers.

2) I would fix this by using the Number() function to convert the strings num1 and num2 into numbers when I add them and store them in result.
