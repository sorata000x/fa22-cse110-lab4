1. ^^^ What will happen at line 12 and why? If the code causes an error, explain why. ^^^
   A: print 3, because when i = prices.length = 3, the for loop exit, and since var variable can be accessed through blocks, 3 is being printed after that.

2. ^^^ What will happen at line 13 and why? If the code causes an error, explain why. ^^^
   A: print 150, similar reason, before i = 3 and for loop exit, i = 2 and discountedPrice = prices[2] * (1 - discount) = 300 * (1 - 0.5) = 150, so when loop exit, 150 is printed.

3. ^^^ What will happen at line 14 and why? If the code causes an error, explain why. ^^^
   A: print 150, because in the loop finalPrice = Math.round(discountedPrice * 100) / 100 = Math.round(150 * 100) / 100 = 150 since var variable can be accessed / modify across scope.

4. ^^^ What will this function return? Give a brief explanation why. If the code causes an error, explain why. ^^^
   A: [50, 100, 150], because each finalPrices are half of the original price, and being pushed into the discounted list one by one.

5. ^^^ What will happen at line 12 and why?  If the code causes an error, explain why. ^^^ (assume this function is being called like the others: discountPrices([100, 200, 300], 0.5)).
   A: error, because i is declared with let keyword in the for loop which is not visible to outer scope, so i doesn't exist for the outer block.

6. ^^^ What will happen at line 13 and why? If the code causes an error, explain why. ^^^
   A: error. Similarly, discountedPrice is declared in the for loop block so cannot be access outside of it.

7. ^^^ What will happen at line 14 and why? If the code causes an error, explain why. ^^^
   A: print 150, because finalPrice is being declared in the same scope as the console.log, so it has no problem accessing it.

8. ^^^ What will this function return? Give a brief explanation. If the code causes an error, explain why. ^^^
   A: [50, 100, 150], since let discounted is being declared at the same level as the return statement, it has no problem accessing it and the values that has been push into it.

9. ^^^ What will happen at line 11 and why? If the code causes an error, explain why. ^^^
   A: error, same issue with #5, it is declared as let in the for loop block.

10. ^^^ What will happen at line 12 and why? If the code causes an error, explain why. ^^^
    A: print 3, because it is a const that being initialized with prices.length = 3, and it is at the same scope as the console.log statement.

11. ^^^ What will this function return? Give a brief explanation. If the code causes an error, explain why. ^^^
    A: print [50, 100, 150], because although a const variable cannot be reassigned, the list is still mutable.

12. Given the above Object, write the notation for:  (These should be in your part2.md)
    A. Accessing the value of the name property in the student object
        - student.name
    B. Accessing the value of the Grad Year property in the student object
        - student['Grad Year']
    C. Calling the function for the greeting property in the student object
        - student.greeting()
    D. Accessing the name property of the object in the Favorite Teacher property in student
        - student['Favorite Teacher'].name
    D. Access index zero in the array of the courseLoad property of the student object
        - student.courseLoad[0]

13. Arithmetic
    A. ‘3’ + 2
        - '32' since integer 2 map to its string representation '2'
    B. ‘3’ - 2
        - 1 since - is numerical operaiton
    C. 3 + null
        - 3 since null map to 0 in numeric
    D. ‘3’ + null
        - 3null since null map to 'null' in string
    E. true + 3
        - 4 since true map to 1 in numeric
    F. false + null
        - 0 since false map to 0 and null is also 0
    G. '3' + undefined
        - 3undefined since undefined amp to 'undefined' in string
    H. '3' - undefined
        - NaN since - is numerical operation and undefined becomes NaN which is not a numerical value

14. Comparison
    A.‘2’ > 1
        - true, string '2' become a number 2
    B.‘2’ < ‘12’
        - false, because the first characters of '12' is '1', which is less than '2', so the '2' is greater than '12'.
    C.2 == ‘2’
        - true, because '2' become number 2
    D.2 === ‘2’
        - false, because === is strict equality and 2 and '2' are different types.
    E.true == 2
        - false, because true become 1 which is not equal to 2.
    F.true === Boolean(2)
        - true, because Boolean(2) become true, which is the same value and type.

15. Explain the difference between the == and === operators.
    == is true if the values are equal.
    === is strict equality which requires both value and type to be equal.

16. Given the above Object, write a for...in loop that will iterate through it and print out the value of the property if the property starts with the letter r, or if the value of that property is an odd number.  (This should be in a JS file part2-question16.js)
    
17. If the function above is called with the following parameters modifyArray([1,2,3], doSomething), what will be the result? Briefly walk through how you arrived at that result. (This should be in your part2.md). Here we are passing in a function as a parameter, however we can also return a function from another function just as easily, you're encouraged to play around with callbacks as they are used heavily in frontend JS development. 
    A: The function call `modifyArray([1,2,3], doSomething)` return a list that is the element-wise multiplied of the input array `[1,2,3]`. In the function `modifyArray` and its for loop, the element of the input array is passed to the callback function `doSomething`, which double the number and return it as the result, which is being pushed into `newArray` for every element of input array and being returned in the end, so the final result is returning [2,4,6] in this case.

18. The above program only prints out the time once when executed. Modify this code such that the program prints out the time every second.  (This should be a JS file - part2-question18.js)

19. What is the output of the above code? (This should be in your part2.md)
    A: 1 4 3 2

